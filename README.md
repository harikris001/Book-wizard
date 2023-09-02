![Chroma Frame](https://github.com/TH-Activities/saturday-hack-night-template/assets/90635335/365c00da-597c-446f-9aa7-bed99fb26074)



# Book - Wizard

## Team Members
1. [Harikrishna R Nair](https://github.com/harikris001)
2. [Alisha Alappat](https://github.com/alishaalappat)

## Video to Product Walkthrough



https://github.com/harikris001/Book-wizard/assets/85405666/3caf105f-bda6-4e4a-8948-89db4daf4231



## How it Works
The LLM (Language Model) Chatbot is designed to interact with users based on the context provided by a PDF document. Here's how it works:

1. **Upload a PDF**: Users can upload a PDF document containing relevant information, such as a research paper or article.

2. **Document Chunking**: The uploaded PDF is split into chunks using the *RecursiveCharacterTextSplitter*.

3. **Embeddings Generation**: The chatbot creates embeddings for each chunk using *SentenceTransformerEmbeddings*.

4. **Vector Store Creation**: A vector store is generated using ChromaDB, allowing for efficient retrieval of context.

5. **Interactive Chat**: Users can then initiate a conversation with the chatbot. The chatbot's responses are generated based on the understanding of the uploaded PDF content, allowing for context-aware interactions.

## Libraries Used
- [langchain](https://python.langchain.com/docs/get_started/introduction.html)
- [pytorch](https://pytorch.org/docs/stable/index.html)
- [chromadb](https://docs.trychroma.com/)
- [transformers](https://huggingface.co/transformers/v3.0.2/index.html)
- [streamlit](https://docs.streamlit.io/)

## How to Configure
To set up the project, follow these instructions:

1. Clone the repository from [GitHub Repo Link](https://github.com/harikris001/Book-wizard).
    ```
    git clone https://github.com/harikris001/Book-wizard.git
    ```
2. Install the required libraries and dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

3. Go To Hugging Face [LaMini-T5-738M](https://huggingface.co/MBZUAI/LaMini-T5-738M) model and download pytorch_model.bin and paste in directory 'LaMini-T5-738M'
4. If you have a GPU with more than 4GB or VRAM recommended to install the CUDA toolkit from Nvidia [CUDA](https://developer.nvidia.com/cuda-toolkit)

## How to Run
To run the LLM Chatbot, follow these steps:

1. Navigate to the project directory:

   ```
   cd Book-wizard
   ```
2. Start the application:
   ```
   streamlit run BookSummarizer_bot.py 
   ```

3. Open your web browser and access the chatbot interface.

4. Upload a PDF document and start chatting with the LLM Chatbot. It will respond based on the context of the uploaded PDF.

Enjoy seamless and context-aware conversations with the LLM Chatbot!

---

Feel free to reach out to our team members if you have any questions or need assistance with the project.

**Disclaimer:** This project is based on a language model, and its performance may vary depending on the complexity and quality of the PDF content provided, performance of the computer etc.
