# API Integration Project

This project integrates with the AlphaVantage API to retrieve daily stock market data for analysis. It uses Python for scripting, SQLite for data storage, and pydantic for data validation.

## Installation

1. Clone the repository:

   `git clone https://github.com/your_username/api-integration-project.git`
  
2. Navigate to the project directory:

   `cd api-integration-project`
   
4. Create a virtual environment and install the required packages:

  `python -m venv venv`
  
  `source venv/bin/activate`  # On Windows, use `venv\Scripts\activate.bat`
  
  `pip install -r requirements.txt`

5. Create a .env file in the project directory with the following format:

        ALPHA_API_KEY=your_api_key_here
        DB_NAME=your_database_name_here
        MODEL_DIRECTORY=your_model_directory_path_here

##Usage
1. Setting Up the Environment

Follow the installation instructions above.
2. Using the API

   -Import the AlphaVantageAPI class from data.py.
   -Create an instance of the AlphaVantageAPI class with your API key.
   -Use the get_daily method to retrieve daily stock market data.

3. Using the Database

    Import the SQLRepository class from data.py.
    Create an instance of the SQLRepository class with a database connection.
    Use the insert_table method to insert data into the database.

4. Additional Notes

    Ensure that the .env file is properly configured with your API key and database information.
    Check the AlphaVantage API documentation for additional query parameters and options.

Testing

   Use unittest framework for testing the project components.
   Write test cases to cover different scenarios such as API call failures, data validation, and database operations.
   Use mock library to simulate API responses and database interactions for testing purposes.
   Run tests regularly to ensure the project's correctness and reliability.

Documentation
[Documentation.pdf]

Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

