### Project Description

*A web app to upload multiple pdfs and ask questions about them to llms (Gemini).*

The backend consists of FastAPI server, which processes and stores the pdfs uploaded in vectore stores. When user asks a doubt, the relevant documents and the entire chat history is provided along with a prompt and the llm responds with relevant output.

### Features

* Supports multiple pdf uploads.
* Follow up questions are easily answered.
  

### Installation

Here's how to install the required dependencies and run the application:

1. **Prerequisites:**
    * Python 3.6+
    * fastapi
    * uvicorn
    * pydantic
    * google-generativeai
    * langchain
    * faiss-cpu

2. **Dependencies:**
    * Install dependencies using a package manager like `pip`:
      ```bash
        pip install -r requirements.txt
        ```
3. **Running the application:**
    * Start the development server:
        ```bash
        cd fastapi
        uvicorn main:app --reload
        ```
    * Access the application in your browser at http://127.0.0.1:8000/


### Usage

Two endpoints used are:

* /uploadfile/ 
* /question/

**Upload pdf:**

The application provides an endpoint to upload multiple pdfs:

```
POST /uploadfile/
```

The uploaded pdfs undergo preprocessing and stored in vector spaces for easy retrieval dring query asking.
This returns a JSON response with a list of filenames corrsponding to the ones uploaded.

**Ask query:**

The application provides an endpoint to ask query related to the documents:

```
POST /question/
```

The question is passed to the llm, along with chat history and a prompt. The llm returns the answer to the query, which is then added to chat history.
This returns a JSON response corrsponding to the updated chat history.

**Deployed at:**

* https://chat-with-pdf-frontend-03q0.onrender.com


