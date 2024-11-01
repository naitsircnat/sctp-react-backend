# Ecommerce Backend API
This is a simple ecommerce backend developed to support the development of a frontend React app.  Do take note that the code here does not represent industry best practices and should not be treated as a "model answer" of sorts.



## Installation Steps

### 1. Clone and Install Dependencies
After cloning, make sure your current working directory is the project directory, and install all dependencies with
```bash
npm install
```

### 2. Database Setup

1. Log into MySQL:
```bash
mysql -u root
```

2. Create a new database:
```sql
CREATE DATABASE react_ecommerce_db;
```

3. Exit the MySQL terminal, and run the following:
```bash
mysql -u root < schema.sql
```

### 3. Configuration

1. Create a `.env` file in the backend directory:

```env
PORT=3000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=
DB_NAME=react_ecommerce_db
```
### 4. Starting the Application

Run the RESTFul API with `node index.js`

Important! If using Gitpod, please ensure that you have set your port to public!

## API Endpoints

### POST /api/register
Registers a new user with the following fields:
- name (string)
- email (string)
- password (string)
- confirmPassword (string)
- salutation (enum: 'Mr', 'Ms', 'Mrs')
- country (enum: 'sg', 'my', 'in', 'th')
- emailMarketing (boolean)
- smsMarketing (boolean)

