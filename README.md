# PERN-stack
## 1) create two folders: client, server

## 2) Beck-end:

In folder server create file index.js
npm install express pg pg-hstore sequelize cors dotenv
npm install -D nodemon // restart server automatically
In settings.json - "scripts" - add "dev": "nodemon index.js"

Create environment: create in server root file .env
in this file:
PORT=5000

### server configuratuon:
In index.js:
require("dotenv").config();  
const express = require('express');  
const PORT = process.env.PORT || 5000;  
const app = express();  
app.listen(PORT, () => console.log(`Server started on port ${PORT}`));  
In terminal - npm run dev

### connect database:
Create in server root file db.js;  

