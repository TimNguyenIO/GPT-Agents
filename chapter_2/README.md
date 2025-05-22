# Chapter 2: GPT Agents

## Introduction
This chapter explores the use of GPT-based agents for building intelligent applications. It demonstrates how to interact with OpenAI's API and manage environment variables securely in Python projects.

## Why
Leveraging GPT agents enables automation, natural language understanding, and advanced AI capabilities in your applications. Using environment variables ensures sensitive information, like API keys, is kept secure and configurable.

## How to Install
1. Install Python (if not already installed):
   - Download the latest version from the [official Python website](https://www.python.org/downloads/).
   - On macOS, you can also use Homebrew:
     ```bash
     brew install python
     ```
2. Verify Python and pip installation:
   ```bash
   python3 --version
   pip3 --version
   ```
3. (Optional) Upgrade pip:
   ```bash
   python3 -m pip install --upgrade pip
   ```
4. Clone this repository or navigate to the `chapter_2` directory.
5. Install the required Python packages:

```bash
pip install -r requirements.txt
```

- `openai`: Official OpenAI Python client for accessing GPT models and other OpenAI services.
- `python-dotenv`: Loads environment variables from a `.env` file, keeping secrets out of your codebase.

### Using a Virtual Environment (Recommended)
To avoid system conflicts and manage dependencies safely, use a virtual environment:

```bash
# Create a virtual environment in your project directory
python3 -m venv venv

# Activate the virtual environment
source venv/bin/activate

# Now install your requirements
pip install -r requirements.txt
```

- This keeps all installed packages isolated to your project.
- To deactivate the environment, run: `deactivate`

## How to Run the Examples
1. Ensure you have followed the installation steps above and activated your virtual environment.
2. Create a `.env` file in the `chapter_2` directory with your OpenAI API key:
   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   ```
3. Run the example script:
   ```bash
   python connecting.py
   ```
   This will send a sample prompt to ChatGPT and print the response.

## References
- [OpenAI Python Library Documentation](https://github.com/openai/openai-python)
- [python-dotenv Documentation](https://pypi.org/project/python-dotenv/)
- See `requirements.txt` for the list of dependencies.
