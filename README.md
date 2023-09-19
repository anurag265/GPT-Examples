# GPT Examples
 Jupyter Notebooks with GPT Examples. Current projects in this repo:
 1. Talk to PDF
 2. Coming Soon.

---

## Talk to PDF

This is a simple chatbot that can look up a given PDF and answer your questions.

### Getting Started

1. Specify the path to the PDF file in the `PDF_FILE_PATH` variable.
2. Run the cells to extract text from the PDF, create embeddings, and prepare the chatbot.
3. Describe your PDF's content and purpose in the `pdf_description` variable.
4. Run the chatbot cell to start interacting.

### Usage

Start an infinite loop, allowing the user to ask questions. To exit, leave the user input blank and hit enter.

### Helper Functions

**1. extract_text_from_pdf**

This function extracts text from the specified PDF file and saves it in a text file (`pdf_text.txt`).

**2. create_embeddings**

This function creates embeddings from the extracted text using OpenAI's embedding model.

**3. get_embeddings**

This function reads the embeddings from the JSON file and prepares them for the chatbot.

**4. user_question_embedding_creator**

This function generates an embedding for the user's question using the specified embedding model.

**5. answer_users_question**

This function answers the user's question based on the provided PDF's search results and the user's input.

### Parameters

Various parameters are specified to configure the behavior of the code, including file paths, API keys, and model choices.

### Notes

- Make sure to replace `OPENAI_API_KEY` with your actual OpenAI API key.
- Adjust the `EMBEDDING_MODEL` and `GPT_MODEL` as needed for your use case.

### Note on Sample Provided

Included a sample PDF file - `chatgpt_unsesco.pdf`. This PDF, titled "ChatGPT and Artificial Intelligence in Higher Education (Quick Start Guide)," is available online under the Open Access license - Attribution-ShareAlike 3.0 IGO (CC-BY-SA 3.0 IGO). You can use this PDF for testing and experimentation purposes.

---

For more details on how to use this code, refer to the comments in the code cells.
