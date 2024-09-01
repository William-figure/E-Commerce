
# E-Commerce 

This project is a backend system for an e-commerce platform built with Node.js, Express, and Sequelize. It provides a RESTful API for managing products, categories, and tags in a SQL database. The application follows the MVC pattern and is structured to handle CRUD operations efficiently.

## Table of Contents

- [E-Commerce](#e-commerce)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Project Structure](#project-structure)
  - [Environment Variables](#environment-variables)
  - [API Endpoints](#api-endpoints)
    - [Categories](#categories)
    - [Products](#products)
    - [Tags](#tags)
  - [Seeding the Database](#seeding-the-database)
  - [Video](#video)

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/William-figure/E-Commerce 
   cd E-COMMERCE
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Set up the database**:

   Ensure you have MySQL installed and a database created for this application. Update your `.env` file with your database credentials.

## Usage

1. **Create a `.env` file** in the root directory with the following contents:

   ```plaintext
   DB_NAME=your_database_name
   DB_USER=your_database_user
   DB_PASSWORD=your_database_password
   ```

2. **Run the application**:

   ```bash
   npm start
   ```

3. **Use API clients like Postman** to test the API endpoints.

## Project Structure

```
E-COMMERCE/
├── config/                 # Database connection configuration
├── db/                     # Database related files
├── models/                 # Sequelize models
├── node_modules/           # Node.js modules
├── routes/                 # Express routes
│   └── api/                # API route handlers
├── seeds/                  # Database seed files
├── .env                    # Environment variables
├── .gitignore              # Git ignore file
├── package.json            # Project configuration and dependencies
├── package-lock.json       # Lockfile for Node.js modules
└── server.js               # Entry point for the application
```

## Environment Variables

The application requires a `.env` file to configure the connection to the SQL database. The following variables should be set:

- `DB_NAME`: Name of the SQL database.
- `DB_USER`: Username for the SQL database.
- `DB_PASSWORD`: Password for the SQL database.

## API Endpoints

### Categories

- **GET** `/api/categories` - Get all categories
- **GET** `/api/categories/:id` - Get a category by ID
- **POST** `/api/categories` - Create a new category
- **PUT** `/api/categories/:id` - Update a category by ID
- **DELETE** `/api/categories/:id` - Delete a category by ID

### Products

- **GET** `/api/products` - Get all products
- **GET** `/api/products/:id` - Get a product by ID
- **POST** `/api/products` - Create a new product
- **PUT** `/api/products/:id` - Update a product by ID
- **DELETE** `/api/products/:id` - Delete a product by ID

### Tags

- **GET** `/api/tags` - Get all tags
- **GET** `/api/tags/:id` - Get a tag by ID
- **POST** `/api/tags` - Create a new tag
- **PUT** `/api/tags/:id` - Update a tag by ID
- **DELETE** `/api/tags/:id` - Delete a tag by ID

## Seeding the Database

To seed the database with initial data, run:

```bash
npm run seed
```

This command will execute the scripts in the `seeds` directory, populating your database with initial data.

## Video
[demo](https://youtu.be/b2_hhc6-MGE)