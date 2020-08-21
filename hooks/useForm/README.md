# useForm hook

#### Basic Usage

``` js
const initialState = { name: '', email: '' }

const [ values, handleInputChange, reset ] = useForm(initialState);

```

```useForm(initialState)``` You can pass an object with all the keys of your form.

!!! You must put a name tag with the correlated key name.

values: an object literal with keys as identifiers of each input.

reset: a function that reset all the values to initial state.

```handleInputChange = ({ target })```: a function that handle all inputs changes.

for example:

``` js
    const initialState = { name: "", email: "" }

    const [ values, handleInputChange ] = useForm( initialState );

    const { name, email, password } = values;

    <form className="form-group ">
      <input
          id="name"
          name="name"
          onChange={ handleInputChange }
          placeholder="Escribe tu nombre"
          type="text"
          value={ name }
      />

      <input
          id="email"
          name="email"
          onChange={ handleInputChange }
          placeholder="Escribe tu e-mail"
          type="text"
          value={ email }
      />
  </form>
```