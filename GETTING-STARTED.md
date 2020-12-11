# Template for getting started

### In the root create file with following Code

```
require('dotenv').config();
const express = require('express');
const app = express();

//sets template engine
app.set('view engine', 'ejs')

//tells to use static files
app.use(express.static('public'))

//makes it possible to use url params
app.use(express.urlencoded({ extended: false }))

app.listen(process.env.PORT, ()=>{
    console.log("start")
})

```
