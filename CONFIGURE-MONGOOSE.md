# Configure Mongoose to connect with mongoDB.


```
const mongoose = require('mongoose');

mongoose.connect('process.env.VARIABLE_NAME', { useNewUrlParser : true })
const db = mongoose.connection
db.on('error', (error) => console.log(error))
db.once('open', ()=> console.log("DB connected successfully"))
```
