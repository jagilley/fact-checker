# fact checking with prompt chaining

This repo is a simple demonstration of using [langchain](https://github.com/hwchase17/langchain) to do fact-checking with prompt chaining. How it works:
- you ask your desired LLM a question
- the LLM generates an initial answer to the question
- the LLM self-interrogates what the assumptions were that went into that answer
- the LLM sequentially determines if each of these assumptions are true
- the LLM generates a new answer to the question, incorporating the new information

## to run

Make sure you have langchain installed (`pip install langchain`). Then run

`python3 fact_checker.py 'insert question here'`

*Be sure to wrap your question in quotes if you're passing it as a command line argument.*

Alternatively, you can use the provided `fact_checker.ipynb` notebook.