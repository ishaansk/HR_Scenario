HR Scenario Q&A App

Overview
This project is a Streamlit-based application that allows users to ask questions about HR-related documents. It uses Groq's Llama3-8b-8192 model to generate responses and employs Google Generative AI Embeddings with FAISS for efficient document retrieval.

 Features
- Streamlit UI: A simple interface for users to input questions.
- Groq Chat Model: Uses `Llama3-8b-8192` to generate answers.
- PDF Document Processing: Loads HR-related PDFs from a directory.
- Google Generative AI Embeddings: Converts text into vector embeddings.
- FAISS Vector Store: Enables fast and accurate document retrieval.
- Real-time Query Processing: Retrieves relevant document chunks and provides AI-generated responses.

 Installation

# 1. Clone the Repository

git clone https://github.com/ishaansk/HR_Scenario
cd HR_Scenario


# 2. Set Up Virtual Environment
```sh
python -m venv myenv2
myenv2\Scripts\activate     # On Windows
```

# 3. Install Dependencies

pip install -r req


# 4. Set Up API Keys
Create a `.env` file in the project root and add your API keys:

GROQ_API_KEY=your_groq_api_key_here
GOOGLE_API_KEY=your_google_api_key_here


 Usage
#5. Run the Streamlit application:

streamlit run app.py


 Folder Structure

HR_Scenario/
├── sources/                  # Folder containing the HR source PDF     
├── app.py                      # Main application script
├── req.txt             # List of dependencies
├── .env                         # API keys (not included in Git)
├── myenv2/                      # Virtual environment (ignored in Git)


 Troubleshooting
- API Key Errors: Ensure `.env` is correctly set up and loaded.
- Module Not Found: Reinstall dependencies using `pip install -r requirements.txt`.
- Vector Embeddings Not Loading: Check if PDFs exist in the `sources` folder.

For a deeper understanding of the concepts and tools involved in the working of this project, visit SOLUTION.md