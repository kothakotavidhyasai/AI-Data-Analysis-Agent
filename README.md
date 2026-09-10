# 🤖 AI Data Analysis Agent

An AI data analysis Agent built using the Agno Agent framework and Google's Gemini 2.5 Flash model. This agent helps users analyze their data (CSV, Excel files) through natural language queries, powered by Google's multimodal language models and DuckDB for efficient data processing - making data analysis accessible to users regardless of their SQL expertise.

## Features

- 📁 **File Upload Support**: Upload CSV and Excel files with automatic data type detection and schema inference.
- 🗣️ **Natural Language Queries**: Convert natural language questions into SQL queries instantly. No SQL knowledge required.
- 📊 **Advanced Analysis**: Perform aggregations, filter data, and generate statistical summaries securely in-memory using DuckDB and Pandas.
- 🔒 **Secure Configuration**: Strictly uses environment variables (`.env`) for API key management, ensuring no secrets are exposed or requested in the UI.
- 💻 **Interactive UI**: User-friendly Streamlit interface for real-time query processing and clear result presentation.

## Prerequisites
- Python 3.9+
- Google Gemini API Key (Get one from [Google AI Studio](https://aistudio.google.com/))

## How to Run

1. **Setup Environment**
   ```bash
   # Clone the repository
   git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
   cd awesome-llm-apps/starter_ai_agents/ai_data_analysis_agent

   # Create a virtual environment (Recommended)
   python -m venv venv
   source venv/bin/activate  # On Windows use: .\venv\Scripts\activate

   # Install dependencies
   pip install -r requirements.txt
   ```

2. **Configure API Keys**
   Create a `.env` file in the root directory of the project and add your Google API key:
   ```env
   GOOGLE_API_KEY="your_google_api_key_here"
   ```
   *Note: The application enforces strict environment-based configuration and will fail to start if this key is missing from the `.env` file.*

3. **Run the Application**
   ```bash
   streamlit run ai_data_analyst.py
   ```

## Usage
1. Launch the application using the command above.
2. Upload your CSV or Excel file through the Streamlit interface.
3. Ask questions about your data in natural language in the query box.
4. View the results, insights, and generated data visualizations directly in the browser!
