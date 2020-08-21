# useFetch hook

#### Basic Usage


``` js

const dataFetched = useFetch( url );

```

```useFetch( url )``` it take a string url.

It will return a data with the next structure:
```js
// start with initial values

{
  data: null, // any data returned
  loading: true, // when the data is fetched it will change to false
  error: null, // If there are some error it will save here
};
  
```
