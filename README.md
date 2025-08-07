# 🤖 Generative AI Notebook for QA Engineers

## Prerequisites

### System Requirements
- **Python**: 3.9 or higher

### Required API Keys

This notebbok uses real AI services and requires the following API keys:

1. **Google Gemini API Key**
   - Sign up at: https://makersuite.google.com/app/apikey
   - Free tier includes generous usage limits
   - Used for: LLM interactions, agent reasoning, content generation

2. **Tavily API Key** 
   - Sign up at: https://tavily.com
   - Free tier includes 1000 searches/month
   - Used for: Real-time web search functionality

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd gen-ai-terminology
   ```

2. **Install dependencies**
   ```bash
   # Using uv (recommended)
   uv sync
   
   # Or using pip
   pip install -e .
   ```

3. **Configure API keys**
   - The `.env` file is already created with placeholders
   - Replace the placeholder values with your actual API keys:
   ```
   GOOGLE_API_KEY=your_actual_google_gemini_api_key
   TAVILY_API_KEY=your_actual_tavily_api_key
   ```

4. **Launch Jupyter (or use VSCode extension to handle this)**
   ```bash
   jupyter notebook main.ipynb
   ```

### Dependencies Overview

The notebook uses the following key libraries:

- **Core AI Libraries**:
  - `langchain` - Framework for building AI applications
  - `langchain-google-genai` - Google Gemini integration
  - `tiktoken` - Token counting and analysis
  - `tavily-python` - Web search functionality

- **Data Science**:
  - `numpy` - Numerical computations
  - `scikit-learn` - Machine learning utilities
  - `matplotlib` - Visualization

- **Utilities**:
  - `python-dotenv` - Environment variable management
  - `requests` - HTTP requests