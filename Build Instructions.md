Stock Price Monitoring System (CS50)

This is a web application built with Python and Flask that allows users to monitor stock prices. This project was developed as part of the CS50 curriculum and utilizes the CS50 library.

Prerequisites

Before you begin, ensure you have the following installed on your system:

Python 3.6 or higher

pip (Python package installer)

Setup and Installation

Follow these steps to get the application running on your local machine.

1. Set up the Environment

It is highly recommended to use a virtual environment to manage project dependencies.

# Create a virtual environment
python3 -m venv venv

# Activate the virtual environment
# On macOS and Linux:
source venv/bin/activate
# On Windows:
.\\venv\\Scripts\\activate


2. Install Dependencies

With your virtual environment activated, install the required packages using the requirements.txt file.

pip install -r requirements.txt


3. Set up API Key

This application requires an API key to fetch stock data. The CS50 projects typically use IEX Cloud.

Sign up for a free account at IEX Cloud.

Navigate to your console to find your publishable API token.

Set the API key as an environment variable in your terminal.

# On macOS and Linux:
export API_KEY="YOUR_API_KEY"

# On Windows (Command Prompt):
set API_KEY="YOUR_API_KEY"

# On Windows (PowerShell):
$env:API_KEY="YOUR_API_KEY"


Note: You must replace "YOUR_API_KEY" with the actual key from your IEX Cloud account. You will need to set this environment variable every time you open a new terminal session.

4. Run the Application

Once the setup is complete, you can run the Flask application.

flask run


The application will start, and you can access it in your web browser at http://127.0.0.1:5000.

Project Structure

.
├── app.py              # Main Flask application file
├── helpers.py          # Helper functions
├── project.db          # SQLite database
├── requirements.txt    # Python dependencies
├── static/             # Static files (CSS, JS, images)
├── templates/          # HTML templates
└── test.py             # Test scripts
