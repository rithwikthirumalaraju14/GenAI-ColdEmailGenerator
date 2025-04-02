# 📧 Cold Mail Generator

## Overview
Cold Mail Generator is a Streamlit web application that scrapes job postings from a given URL, extracts job details using a GROQ-powered LLM, and generates personalized cold emails with relevant portfolio links. The application leverages ChromaDB for portfolio retrieval and LangChain for LLM interactions.

## Features
- Scrapes job descriptions from career pages.
- Extracts key details like role, experience, skills, and description.
- Matches job requirements with relevant portfolio links using ChromaDB.
- Generates professional cold emails tailored to the job posting.

## Tech Stack
- **Streamlit** - Web UI framework
- **LangChain** - For LLM-powered job extraction and email generation
- **ChatGroq (LLM)** - Handles text processing and generation
- **ChromaDB** - Vector database for portfolio matching
- **Pandas** - Data manipulation
- **Regex (re)** - Text cleaning and preprocessing

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/cold-mail-generator.git
   cd cold-mail-generator
   ```

2. Create a virtual environment and install dependencies:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   ```

3. Set up environment variables:
   - Create a `.env` file and add your **GROQ_API_KEY**:
   ```sh
   GROQ_API_KEY=your_api_key_here
   ```

## Usage

Run the Streamlit application:
```sh
streamlit run app.py
```

### How It Works
1. Enter a job posting URL.
2. Click **Submit** to scrape and extract job details.
3. The LLM processes the job details and retrieves relevant portfolio links.
4. A personalized cold email is generated and displayed.

## File Structure
```
.
├── app.py                  # Main Streamlit app
├── chains.py               # Handles LLM-based job extraction & email writing
├── portfolio.py            # ChromaDB integration for portfolio retrieval
├── utils.py                # Text cleaning utilities
├── requirements.txt        # Python dependencies
├── resource/
│   ├── my_portfolio.csv    # Portfolio data with tech stack and links
├── .env                    # API key for GROQ LLM
└── README.md               # Project documentation
```

## License
This project is licensed under the MIT License.

## Contact
For any inquiries, contact **Rithwik** at [rithwik.t2003@gmail.com](mailto:rithwik.t2003@gmail.com).

