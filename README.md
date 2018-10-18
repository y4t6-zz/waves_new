# SERVER PART

Install nodemon

```
npm install -g nodemon
```

Create directories: */client* and */server*
Install dependencies:

```
npm install bcrypt@2.0.1 body-parser@1.18.3 cloudinary@1.11.0 concurrently@3.6.0 cookie-parser@1.4.3 dotenv@6.0.0 express@4.16.3 express-formidable@1.0.0 jsonwebtoken@8.3.0 moment@2.22.2 mongoose@5.1.6 multer@1.3.0 --save
```
- Create file /server/server.js
- Add script to package.json

```
"start": "node server/server.js",
"server": "nodemon server/server.js"
```

Add script to /server/server.js


```javascript
const express = require('express');

const app = express();

const port = process.env.PORT || 3002;

app.listen(port, ()=>{
   console.log(`Server Running at ${port}`)
});
```
