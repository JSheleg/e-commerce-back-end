# E-commerce Back End ![Github licence](http://img.shields.io/badge/license-MIT-blue.svg)

## Description:

Command Terminal applicatioon that uses `express` and `sequelize` to build the back end of an e-commerce site. 

## Table of Contents:

* [User Story](#user-story)
* [Acceptance](#acceptance)
* [Installation](#installation)
* [Instructions](#instructions)
* [Database Models](#database-models)
* [API Routes](#api-routes)
* [License](#license)
* [Questions](#questions)
* [Walk Through](#walk-through)


## User Story

```md
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies
```

## Acceptance

```md
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database
```
## Installation
* Clone Repo from GitHub and run `git clone <url copied from repository> `
* `npm install`

## Instructions
* To start the program run:
    `npm start` or `node server.js`
* To quit the program:
    `CTRL + C` 
* Login in to MySql
    Run `mysql -u root -p ` in terminal and input password from .env file.
* Run Schema and seed data
    `source db/schema.sql` 
* Quit and seed data:  `npm run seed`


## Database Models

Database models will include: 

* `Category`
  * `id`
  * `category_name`

* `Product`
  * `id`
  * `product_name`
  * `price`
  * `stock`
  * `category_id`

* `Tag`
  * `id`
  * `tag_name`

* `ProductTag`
  * `id`
  * `product_id`
  * `tag_id`


## API Routes

* `Routes( Category, Product and Tag )`
  * `Create`
  * `FindAll`
  * `FindOne`
  * `Update`
  * `Destroy`

## License

This project is licensed under MIT

## Questions
* Created by Jessica Sheleg
* [Project Repository](https://github.com/JSheleg/e-commerce-back-end)
* [GitHub Portfolio](https://github.com/JSheleg)

## Walk Through
* [MySql and Seeding Data]()
* [Categories]()
* [Products]()
* [Tags]()
