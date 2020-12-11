# How to create Routes folder and template

* Go to root and create folder by name **routes**
* In **routes folder** create file for routes and add following code.
```
const router = require('express').Router();

//Home Route
router.get('/', (req, res)=>{
  res.send('success')
})


module.exports = router;
```
