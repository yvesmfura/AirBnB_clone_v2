# Airbnb Clone Project V2

## Introduction
Welcome to our Airbnb Clone project! This project aims to replicate the functionality of the popular Airbnb platform using Python and SQLAlchemy for database management and modeling. Whether you're a traveler looking for accommodation or a host wanting to list your property, our clone project provides a seamless experience.

## Features
- **User Management**: Create, update, and delete user accounts.
- **Property Listing**: Hosts can list their properties with detailed descriptions and amenities.
- **Reviews**: Guests can leave reviews for properties they've stayed in.
- **Search Functionality**: Users can search for properties based on location, price, and amenities.
- **Environment Configuration**: Flexible environment variables for easy configuration.

## Learning Objectives
By working on this project, you will gain experience in:
- Implementing Unit Testing in a large project.
- Utilizing *args and **kwargs effectively in Python.
- Managing a MySQL database and understanding ORM.
- Utilizing environment variables for configuration.

## Requirements
### Python Scripts:
- Compatible editors: vi, vim, emacs.
- Interpretation/Compilation on Ubuntu 20.04 LTS using Python 3.8.5.
- Follow PEP8 styling guidelines using `pycodestyle`.
- All files must be executable.
- Use descriptive documentation for modules, classes, and functions.
- Utilize environment variables for configuration.

### Python Unit Tests:
- Utilize the `unittest` module.
- Organize test files within a `tests` folder.
- Execute tests using `python3 -m unittest discover tests`.

### SQL Scripts:
- Executed on Ubuntu 20.04 LTS using MySQL 8.0.
- Use SQLAlchemy version 1.4.x for Object-Relational Mapping.
- Follow SQL best practices and conventions.
- End all files with a new line.

## Getting Started
To get started with our Airbnb Clone project, follow these steps:
1. **Clone the Repository**: `git clone <repository-url>`
2. **Set Up MySQL Database**: Configure MySQL database settings using environment variables.
3. **Install Dependencies**: Ensure you have all required dependencies installed.
4. **Start Coding**: Dive into the code and start building your Airbnb clone!

## Project Structure
Our project follows a structured approach with models for User, Place, Review, Amenity, and City. Additionally, we have test scripts to ensure the functionality of our project remains intact.

## Usage
Here's how you can run the project:
1. **Clone the Repository**: `git clone <repository-url>`
2. **Navigate to Project Directory**: `cd airbnb-clone`
3. **Execute Test Script**: Run `main_place_amenities.py` to demonstrate the Many-to-Many relationship between Place and Amenity.

## Contributions
This project was made possible by the collaborative efforts of our team:
1. **Twayinganyiki LEONCE**
2. **Yves IRAKOZE MFURA**

We welcome contributions from the community to enhance and improve our Airbnb Clone project. Feel free to fork the repository, make changes, and submit pull requests.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
