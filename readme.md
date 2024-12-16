# Magazine Author Article Database Application
 # Overview
This application provides functionality to manage articles, authors, and magazines using a relational database. The user can add authors, magazines, and articles to a database, and the application will display all the records. The project demonstrates the interaction between the Python application and a SQLite database.

 # Key Components
  Author: Represents the authors of the articles, including their name and the articles they have written.
  Magazine: Represents the magazines where articles are published, including the magazine’s name, category, and the articles it contains.
  Article: Represents the articles written by authors and published in magazines. Each article contains a title, content, author ID, and magazine ID.
# Database Tables
The application interacts with three database tables:

authors: Stores information about the authors (id, name).
magazines: Stores information about the magazines (id, name, category).
articles: Stores information about the articles (id, title, content, author_id, magazine_id).
 # Requirements
Python 3.x
SQLite3 (or any other database compatible with SQL commands)
# To run the application, you'll need to set up the environment with the necessary packages (if not already installed):

pip install sqlite3


# Setup Instructions
Clone the repository: If you're working with the GitHub repository:


git clone <git@github.com:Jose-Barasa1/Moringa-FT09-phase-3-code-challenge.git>
cd <Moringa-FT09-phase-3-code-challenge>
Run the Setup Script: The setup.py script contains the function create_tables() that sets up the necessary tables for the application. This function should be run once to initialize the database.

# Run this from a Python environment:


python database/setup.py


# Enter User Input:
The application will prompt you to enter details for an author, magazine, and article:

Author's name
Magazine name
Magazine category
Article title
Article content

# The script will create records in the database for:

Author: Adds the author to the authors table.
Magazine: Adds the magazine to the magazines table.
Article: Adds the article to the articles table with foreign keys to the author and magazine.
Display Data:
After adding the records, the script will fetch all records from the database and display them in a readable format:


# Future Improvements
Input Validation: Add more robust validation for user input to ensure valid data entry (e.g., checking for empty content in articles).
Error Handling: Implement error handling for database operations, such as invalid queries or connection errors.
Model Refactor: Move SQL queries into model methods (currently, they are embedded in main.py).

# License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contact
If you have any questions or suggestions, feel free to reach out. 
 <jose.barasa@student.moringaschool.com/>

