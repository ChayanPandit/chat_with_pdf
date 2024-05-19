### Project Description

*A web app to upload multiple pdfs and ask questions about them to llms (Gemini).*

The backend consists of FastAPI server, which processes and stores the pdfs uploaded in vectore stores. When user asks a doubt, the relevant documents and the entire chat history is provided along with a prompt and the llm responds with relevant output.

### Features

* Supports multiple pdf uploads.
* Follow up questions are easily answered.

This section can include details about functionalities, supported data models, or unique aspects of the app.

### Installation

Here's how to install the required dependencies and run the application:

1. **Prerequisites:**
    * Python 3.6+
2. **Dependencies:**
    * Install dependencies using a package manager like `poetry`:
        ```bash
        poetry install
        ```
3. **Running the application:**
    * Start the development server:
        ```bash
        poetry run uvicorn main:app --reload
        ```
    * Access the application in your browser at http://127.0.0.1:8000/

**Note:** These are general instructions. You might need to modify them based on your specific project setup.

### Usage

This section details how to interact with the application's API. It can include:

* Instructions on using the API endpoints. 
* Examples of API requests with expected responses.
* Links to any generated API documentation (Swagger UI, ReDoc).

**Example:**

The application provides an endpoint to retrieve a list of items:

```
GET /items/
```

This returns a JSON response with a list of items.

**Additional Documentation:**

* Consider including links to any additional documentation you might have, like code explanations or deployment instructions.

### Contributing

* If you'd like people to contribute to your project, outline your contribution guidelines here.

This section can specify preferred ways for users to submit bug reports, feature requests, or code contributions.

### License

* Specify the license under which your code is distributed.

You can mention the license name and provide a link to the license text file.

**Please note:** This is a template. You should customize it to fit your specific FastAPI application.
