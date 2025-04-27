# Setting Up Your OpenAI API Key

To use this email agent, you need to have an OpenAI API key. Follow these steps to set it up:

## Option 1: Environment Variable (Recommended)

1. Get your API key from the [OpenAI dashboard](https://platform.openai.com/api-keys)
2. Set it as an environment variable:

   **Linux/macOS:**
   ```bash
   export OPENAI_API_KEY="your-api-key-here"
   ```

   **Windows (Command Prompt):**
   ```cmd
   set OPENAI_API_KEY=your-api-key-here
   ```

   **Windows (PowerShell):**
   ```powershell
   $env:OPENAI_API_KEY = "your-api-key-here"
   ```

3. Run the email agent:
   ```bash
   python email-agent.py
   ```

## Option 2: Configuration File

1. Create a file named `.env` in the project directory:
   ```
   OPENAI_API_KEY=your-api-key-here
   ```

2. Install python-dotenv:
   ```bash
   pip install python-dotenv
   ```

3. Modify the email-agent.py file to load from dotenv:
   ```python
   from dotenv import load_dotenv
   load_dotenv()  # Add this near the top of the file
   ```

**Important:** Never commit your API key to version control. The `.env` file is already included in the .gitignore file. 