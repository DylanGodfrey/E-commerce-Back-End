# E-Commerce Back End

## Description
To remain competitive in today's market, this e-commerce back-end uses the latest technologies to perform CRUD operations on a database. Built using MySQL2, Express and Sequelize. Recommended to use with Postman or Insomnia API Clients.

![Screenshot of finished project in Insomnia](assets/images/samplescreenshot.png)

Link to Video Example: https://drive.google.com/file/d/1yTb8Kthv6klL9VFyrfR6QRt-dVP6oLcl/view

## Installation

To install, clone the repo:
```
git clone https://github.com/DylanGodfrey/E-commerce-Back-End
```
This project relies on the MySQL2, Express and Sequelize packages:
```
npm install mysql2 express sequelize
```
For security, access to the database info is stored in an .env file, create your own with:
```
echo "DB_NAME='ecommerce_db'" >> .env;
echo "DB_USER='MYSQL USERNAME'" >> .env;
echo "DB_PASSWORD='MYSQL PASSWORD'" >> .env;
```

## Usage

First, the MySQL database must set up using your login credentials:

Run the following command in a terminal at the root of your project:
```
mysql -u <MYSQL USERNAME> -p
```
Enter your password when prompted
```
source db/schema.sql
```
```
quit
```
(optional)Then, initialize the database with seed values:
```
node seed
```
Finally, start the server:
```
npm start
```

This will launch the Express server on localhost:3001. A user can then use their preferred API Client to perform CRUD operations on the database using the corresponding endpoints (refer to routes/api files for full list of supported operations).

## MIT License

Copyright (c) 2022 DylanGodfrey

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
