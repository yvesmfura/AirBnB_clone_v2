# Airbnb Clone Project

## Introduction
This project is a Python-based clone of the popular Airbnb platform. It utilizes SQLAlchemy for database storage and modeling. Below are the key updates and features implemented based on the provided information:
#!/usr/bin/python3
"""
0x02 AirBnB clone - MySQL

Project Description:
This project is a group effort to develop an AirBnB clone using MySQL as the database backend. The project is implemented in Python and follows Object-Oriented Programming (OOP) principles. It involves working with SQL, specifically MySQL, and utilizing ORM (Object-Relational Mapping) with SQLAlchemy. Environment variables are utilized for configuration, providing flexibility in different environments.

Environment Variables:
To configure the project, the following environment variables are utilized:

- HBNB_ENV: Running environment. Can be set to "dev" or "test" for development and testing environments respectively.
- HBNB_MYSQL_USER: MySQL username.
- HBNB_MYSQL_PWD: MySQL password.
- HBNB_MYSQL_HOST: MySQL hostname.
- HBNB_MYSQL_DB: MySQL database name.
- HBNB_TYPE_STORAGE: Type of storage used. Can be set to "file" (using FileStorage) or "db" (using DBStorage).

Learning Objectives:
Upon completion of this project, you should be able to:

- Explain Unit testing and implement it in a large project.
- Understand and utilize *args and **kwargs in Python.
- Handle named arguments in functions effectively.
- Create and manage a MySQL database.
- Create a MySQL user and grant privileges.
- Understand ORM and map Python classes to MySQL tables.
- Manage two different storage engines using the same codebase.
- Utilize environment variables effectively for configuration.

Requirements:
Python Scripts:
- Use editors: vi, vim, emacs.
- All files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.5).
- End all files with a new line.
- The first line of all files should be #!/usr/bin/python3.
- Include a README.md file at the root of the project folder.
- Use pycodestyle (version 2.8.*) for code formatting.
- All files must be executable.
- Test file lengths using wc.
- All modules, classes, and functions should have documentation.
- Documentation should be descriptive and not just a single word.

Python Unit Tests:
- Use editors: vi, vim, emacs.
- All files should end with a new line.
- Place all test files inside a folder named tests.
- Utilize the unittest module.
- Test files should have a .py extension.
- All test files and folders should start with test_.
- Organize test files in a similar structure as the project files.
- Execute all tests using python3 -m unittest discover tests.
- Ensure all modules, classes, and functions have documentation.
- Collaborate on test cases to cover edge cases effectively.

SQL Scripts:
- Use editors: vi, vim, emacs.
- All files will be executed on Ubuntu 20.04 LTS using MySQL 8.0.
- Use SQLAlchemy version 1.4.x.
- End all files with a new line.
- Add comments before SQL queries.
- Start files with a comment describing the task.
- Use uppercase for all SQL keywords.
- Include a README.md file at the root of the project folder.
- Test file lengths using wc.

Getting Started:
To get started with this project, follow these steps:

1. Clone the repository.
2. Set up your MySQL database and configure environment variables accordingly.
3. Ensure you have the required dependencies installed.
4. Start coding!
"""

## Updates Made

### 1. Update User Model
- Added class attributes for `email`, `password`, `first_name`, and `last_name`.
- Specified constraints such as maximum character length and nullability.
- Implemented creation of User objects with specified attributes.

### 2. Update Place Model
- Added class attributes for various place details such as `city_id`, `user_id`, `name`, `description`, etc.
- Specified constraints and default values for certain attributes.
- Implemented creation of Place objects with specified attributes.

### 3. Update User and City Models
- Established relationships between User and Place, and City and Place models.
- Defined relationships such that when a User or City object is deleted, all linked Place objects are automatically deleted.

### 4. Update Review Model
- Added class attributes for `text`, `place_id`, and `user_id`.
- Specified constraints and foreign key relationships.
- Implemented creation of Review objects with specified attributes.

### 5. Update User and Place Models (Continued)
- Added or replaced class attributes to establish relationships with the Review model.
- Defined relationships such that when a User object is deleted, all linked Review objects are automatically deleted.

### 6. Update Amenity Model
- Added class attributes for `name`.
- Established a Many-to-Many relationship between Place and Amenity.
- Created a separate table called `place_amenity` to manage the relationship.
- Implemented the relationship for both DBStorage and FileStorage engines.

### 7. Test Script - `main_place_amenities.py`
- Created a test script to demonstrate the Many-to-Many relationship between Place and Amenity.
- The script creates instances of State, City, User, Place, and Amenity, and establishes relationships between them.

## Project Structure
The project directory structure includes models for User, Place, Review, Amenity, and City, along with test scripts and a README file.

## Database Schema
The database schema consists of multiple tables representing various entities such as users, places, reviews, amenities, etc. Relationships between these entities are established using foreign keys and Many-to-Many relationships.

## Usage
To run the project:
1. Clone the repository.
2. Navigate to the project directory.
3. Execute the test script (`main_place_amenities.py`) to demonstrate the Many-to-Many relationship between Place and Amenity.

## Conclusion
This Airbnb clone project provides a comprehensive demonstration of database storage and modeling techniques using Python and SQLAlchemy. With features such as user management, property listing, reviews, and amenities, the project closely mimics the functionality of the Airbnb platform.

## Contributors
This project was made possible by the collaborative efforts of our team:

## 1.Twayinganyiki LEONCE
## 2.Yves IRAKOZE MFURA
