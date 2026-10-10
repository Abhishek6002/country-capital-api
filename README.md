Country Capital API
Overview

The country-capital-api is a REST API built with Python and Flask that returns the name of a country when a capital city is provided.

The API is served using Uvicorn and is available as a microservice endpoint for other projects to consume:

https://example.com/country-capital/<query-params>

Prerequisites

Before setting up the project locally, ensure you have the following installed:

Python 3.9 or a compatible version supported by the project.
pip, Python's package installer.
Git, to clone the repository.
A terminal or command-line interface.


Local Development Setup
1. Clone the repository
git clone <repository-url>
cd country-capital-api


Replace <repository-url> with the actual Git repository URL.

2. Create a virtual environment
python -m venv .venv


Activate the virtual environment.

macOS/Linux:

source .venv/bin/activate


Windows:

.venv\Scripts\activate

3. Install dependencies

If the repository contains a requirements.txt file, install the dependencies with:

pip install -r requirements.txt


Ensure that Flask and Uvicorn are installed as required by the project.

4. Start the API locally

Run the project's documented Uvicorn startup command. For example, if the application exposes a compatible ASGI application as app in main.py, the command may be:

uvicorn main:app --reload


Adjust the module and application names to match the repository configuration.

5. Access the API

Once the API is running, send a request to its configured local endpoint, using the appropriate query parameters.

The organization-provided microservice endpoint is:

https://example.com/country-capital/<query-params>

Replace <query-params> with the parameter format expected by the API.

Refer to the project's route definitions or API documentation for the exact request format and available local URL.

Notes
Use the Python version and dependency versions specified by the project, if available.
Do not commit virtual environments or local environment configuration files to version control.
Follow the repository's existing setup instructions if they differ from the examples above.
