
# Chat with PDF

A Simple Chatbot which gives answers to the questions asked only on the basis of the PDFs uploaded, with the help of [Google's Gemini LLM model](https://ai.google.dev/gemini-api/docs).    
No Non-Sense Generated, only relevant information provided !!!  
A user can upload multiple PDF files at a time, with size of upto 200 MB.  
Built using [Langchain](https://python.langchain.com/docs/get_started/introduction/) which helps to monitor the performance of Gemini using [LangSmith](https://python.langchain.com/docs/langsmith/).


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file.  
Create a .env file in the root directory of your project and add the following values

`GEMINI_PRO_API_KEY = "YOUR_API_KEY"`

`LANGCHAIN_API_KEY = "YOUR_API_KEY"`

`LANGCHAIN_PROJECT = "NAME_OF_YOUR_PROJECT"`

The LANGCHAIN_PROJECT variable is used to create a new project named NAME_OF_YOUR_PROJECT which is then observable in LangSmith.  
If you do not want to create a project in LangSmith and only want to use LangChain as a framework then you may ignore the variables `LANGCHAIN_API_KEY` & `LANGCHAIN_PROJECT`.
## Run Locally

Clone the project

```bash
  git clone https://link-to-project
```

Go to the project directory

```bash
  cd my-project
```

Install dependencies

```bash
  pip install -r requirements.txt
```

Start the server

```bash
  streamlit run app.py
```


## Note

A folder named faiss_index will be generated which stores vector format of the texts in the PDF files uploaded. 

