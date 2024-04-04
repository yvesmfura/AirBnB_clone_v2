# HBNB - AirBnB Clone

[![CodeStyle](https://github.com/B3zaleel/AirBnB_clone_v2/actions/workflows/codestyle.yml/badge.svg)](https://github.com/B3zaleel/AirBnB_clone_v2/actions/workflows/codestyle.yml)

## Overview

Welcome to HBNB, the AirBnB Clone project. This repository serves as the foundation for a student project aimed at replicating the functionality of the AirBnB website. At its current stage, the project focuses on building a backend interface, or console, facilitating the management of program data. Through the console, users can create, update, and delete objects, as well as manage file storage. The system ensures persistent storage between sessions by employing JSON serialization/deserialization.

---

## The Command Interpreter

The Command Interpreter provides a straightforward REPL (Read-Evaluate-Print-Loop) for interacting with the project's models. It not only serves to test the functionality of supported storage engines but also allows users to manipulate data efficiently. Below, you'll find details on how to use the Command Interpreter, supported commands, and examples of their usage.

### Usage Instructions

1. Clone this repository to your local environment.
2. Navigate to the cloned directory and locate the "[console.py](console.py)" file.
3. Run the console.py file as follows:
   ```bash
   ./console.py


Supported Commands
The following table outlines the supported commands along with their descriptions:

Command Format	Description
help [command]	Prints helpful information about a specific command. If no command is provided, it prints the help menu.
quit	Closes the command interpreter.
EOF	Closes the command interpreter.
create Model [prop_key=prop_value]...	Creates a new instance of the specified model class with the given properties.
count Model	Prints the number of instances of the specified model class.
show Model id	Prints the string representation of an instance of the specified model class with the given ID.
destroy Model id	Deletes an instance of the specified model class with the given ID.
all [Model]	Prints a list containing the string representation of all instances of the specified model class. If no model is provided, all available objects are printed.
update Model id attr_name attr_value	Updates an instance of the specified model class with the given ID by assigning the attribute value to its attribute named attr_name.
update Model id dict_repr	Updates an instance of the specified model class with the given ID by storing the key-value pairs in the provided dictionary as its attributes.
Supported Models
The project supports the following models:

Class	Description
BaseModel	An abstract class representing the base class for all models.
User	Represents a user account.
State	Represents the geographical state in which a User lives or a City belongs to.
City	Represents an urban area in a State.
Amenity	Represents a useful feature of a Place.
Place	Represents a building containing rooms that can be rented by a User.
Review	Represents a review of a Place.
Environment Variables
The project utilizes several environment variables for configuration:

HBNB_ENV: The running environment, which can be dev or test.
HBNB_MYSQL_USER: The MySQL server username.
HBNB_MYSQL_PWD: The MySQL server password.
HBNB_MYSQL_HOST: The MySQL server hostname.
HBNB_MYSQL_DB: The MySQL server database name.
HBNB_TYPE_STORAGE: The type of storage used, which can be file (using FileStorage) or db (using DBStorage).
