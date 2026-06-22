# LangChain Tutorials - Krish Naik Course

This repository contains a collection of Jupyter Notebooks demonstrating various core concepts of **LangChain**, following tutorials inspired by Krish Naik. The tutorials cover building intelligent LLM-based agents, structured outputs, managing message histories, and using custom tools with model providers like Google Gemini, OpenAI, and Groq.

## 🚀 Repository Contents

The project is structured under the `LangChain/` directory:

1. **[1-LangChainIntro.ipynb](file:///d:/AI%20Material/LangChain-Krish%20Naik/LangChain/1-LangChainIntro.ipynb)**
   - Introduction to LangChain concepts.
   - Initializing chat models using Google Generative AI (`ChatGoogleGenerativeAI`).
   - Building and invoking basic conversational agents with custom tools (e.g., weather fetching tool).

2. **[2-ModelInteration.ipynb](file:///d:/AI%20Material/LangChain-Krish%20Naik/LangChain/2-ModelInteration.ipynb)**
   - Interacting directly with language models.
   - Comparing outputs and configuring model-specific parameters.

3. **[3-tools.ipynb](file:///d:/AI%20Material/LangChain-Krish%20Naik/LangChain/3-tools.ipynb)**
   - Creating, binding, and executing custom LangChain tools.
   - Equipping agents with custom capabilities.

4. **[4-messages.ipynb](file:///d:/AI%20Material/LangChain-Krish%20Naik/LangChain/4-messages.ipynb)**
   - Managing chat messages (System, Human, and AI messages).
   - Structuring conversation histories for contextual dialogue.

5. **[5-structuredoutput.ipynb](file:///d:/AI%20Material/LangChain-Krish%20Naik/LangChain/5-structuredoutput.ipynb)**
   - Defining and requesting structured outputs (e.g., JSON schemas or Pydantic objects) from LLMs.

6. **[6-middleware.ipynb](file:///d:/AI%20Material/LangChain-Krish%20Naik/LangChain/6-middleware.ipynb)**
   - Implementing middleware, custom callback handlers, and run tracing in LangChain.

---

## 🛠️ Tech Stack & Dependencies

The project is configured using Python 3.14+ (or equivalent Python version) with `pyproject.toml` and lock files handled by [uv](https://github.com/astral-sh/uv).

Core libraries utilized:
- **LangChain Core & Community**: `langchain`, `langchain-community`
- **Google GenAI / VertexAI**: `langchain-google-genai`, `langchain-google-vertexai` (Gemini model integrations)
- **OpenAI & Groq**: `langchain-openai`, `langchain-groq`
- **Environment Management**: `python-dotenv`
- **Notebook Environment**: `ipykernel`

---

## 💻 Setup and Installation

### 1. Prerequisites
Ensure you have Python installed. We recommend installing `uv` for lightning-fast package management:
```bash
# Install uv (macOS/Linux)
curl -LsSf https://astral.sh/uv/install.sh | sh

# Install uv (Windows PowerShell)
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```

### 2. Install Dependencies
Run the following to initialize the virtual environment and install the required libraries:
```bash
# Using uv (Recommended)
uv sync

# Or using standard pip
python -m venv .venv
source .venv/bin/activate  # On Windows use: .venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Environment Variables
Create a `.env` file in the root directory and add your API keys:
```env
GOOGLE_API_KEY=your_gemini_api_key_here
OPENAI_API_KEY=your_openai_api_key_here
GROQ_API_KEY=your_groq_api_key_here
```
> **Note**: `.env` is listed in `.gitignore` to prevent secret leaks to your GitHub repository.

---

## 📈 Running the Notebooks

Launch the notebook interface inside the virtual environment:
```bash
# Using uv
uv run jupyter lab

# Or standard activation
jupyter notebook
```
Select the virtual environment kernel (`.venv`) when running cells.
