# E-commerce-backEnd
build the back end for an e-commerce site. 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


## Table of Contents
- [Technology](#technology)
- [Installation](#installation)
- [Usage](#usage)
- [Demonstration](#demonstration)
- [Questions](#questions)

## Technology
[MySQL2](https://www.npmjs.com/package/mysql2) and [Sequelize](https://www.npmjs.com/package/sequelize) packages to connect your Express.js API to a MySQL database and the [dotenv](https://www.npmjs.com/package/dotenv) package to use environment variables to store sensitive data.


## Installation
Install npm package that it need by using the following command:
```bash
npm install
```
Check package.json to see what has been installed
```
   "dependencies": {
    "dotenv": "^8.2.0",
    "express": "^4.17.1",
    "mysql2": "^2.1.0",
    "sequelize": "^5.21.7"
  }
```
Create a .env file in the root of this project:
```
DB_NAME='ecommerce_db' . //db name
DB_USER=''   // set your user name     
DB_PASSWORD=''  //set your password
```

## Usage

Firstly, Create database tables by using the following command.
```zsh
mysql -u root -p  
source db/schema.sql
quit
```
Seed data to your database
```zsh
npm run seed
```
Start the application by using the following command.
```zsh
npm start
```
Application Flow
```
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia
THEN I am able to successfully create, update, and delete data in my database
```

## Demonstration
[ViewDemoVideo](https://drive.google.com/file/d/1CPVQ2g3GbMeNzdnCdnNiBjegBsTyuvyz/view)

## Questions
if you have more question, reach me out below.
* Github repository : https://github.com/rogseo
* email : rogseo@gmail.com
