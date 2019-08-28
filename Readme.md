# Initiatives

use babel-plugin as the middlware to catch cases like 

```js
try{
  // try to do
}catch (e){
  // catch block like this
  console.log(e); 
}
```
transform the above code to
```js
try{
  // try to do
}catch (e){
  // catch block like this
  console.log(e); 
  throw e;
}
```

# Test
`npx jest test/`
