# input_integer_state_version

```bash
1. create index.html file 
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
</head>
<body>
    <script src="bundle.js"></script>
</body>
</html>
2. npm init follow the procedure  
2. npm install budo --save -dev // start a server with a default index.html and incrementally bundle your source on filesave
3. add .gitignore file 
4. add /node_modules in it 
5. create src folder add index.js into it as it is our child module because it would be used by other module so we would add 
module.exports = input_integer
```


```bash
When git clone do npm install to install dependency
```

## Initialization
For every module that uses the STATE management library, the first three lines are almost same:

```js
const STATE = require('STATE')
const statedb = STATE(__filename)
const { sdb, get } = statedb(fallback_module)

```