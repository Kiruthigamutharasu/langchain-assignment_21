

## Assignment 21 – LangChain Document Loaders and Text Splitters

### Project Overview

This assignment demonstrates the usage of LangChain document loaders and text splitters for processing unstructured data. The objective is to load documents from multiple sources, split them into manageable chunks, and understand how preprocessing supports Retrieval Augmented Generation (RAG) workflows. No vector database or LLM integration is used as per the assignment requirements.




### Implemented Tasks

#### Part 1 – Document Loaders

1. **TextLoader** – Loaded content from a plain text file and displayed page content and metadata.
2. **CSVLoader** – Converted each row of a CSV file into individual documents.
3. **PyPDFLoader** – Extracted text from a multi-page PDF file.
4. **DirectoryLoader** – Loaded multiple file types from a directory using appropriate loaders.
5. **WebBaseLoader** – Retrieved and processed content from a public webpage.

#### Part 2 – Text Splitters

6. Explained the need for splitting large documents before sending them to language models.
7. Implemented **CharacterTextSplitter** for length-based chunking.
8. Implemented **RecursiveCharacterTextSplitter** for structure-aware splitting.
9. Described semantic chunking concepts and advantages.
10. Discussed how different splitters affect retrieval quality.

#### Part 3 – Mini Integration

11. Created a unified function that selects the correct loader based on file type and performs splitting.
12. Documented observations regarding loader selection, chunk size, and overlap.


### Installation

Run the following commands before executing the notebook:

```
pip install langchain
pip install langchain-community
pip install langchain-text-splitters
pip install pypdf
pip install unstructured
```



### How to Run

1. Place all sample files inside the **data/** folder.
2. Open **assignment21.ipynb** in Jupyter Notebook or Google Colab.
3. Execute cells sequentially from top to bottom.
4. Verify printed outputs for each task.



### Key Learnings

* Different file formats require dedicated document loaders.
* Large documents must be split to respect model token limits.
* Chunk size and overlap significantly influence retrieval performance.
* Recursive splitting preserves semantic structure better than simple length-based methods.



### Tools and Libraries

* LangChain Community Loaders
* LangChain Text Splitters
* PyPDF
* Unstructured
* Jupyter Notebook


