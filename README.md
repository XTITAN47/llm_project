# LLM Project

An experimental LLM chatbot project with a Gradio interface and Hugging Face
Inference API integration.

## Project structure

- `llm_project/app.py` - Gradio chatbot application.
- `src/llm_project/` - reusable project modules.
- `tests/` - project tests.
- `artifacts/` - generated logs and other local artifacts.

## Requirements

- Python 3.10 or newer
- A Hugging Face account and access to the configured inference model

## Setup

Create and activate a virtual environment, then install the application
dependencies:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install gradio huggingface_hub
```

## Run the chatbot

From the repository root:

```powershell
python llm_project\app.py
```

Open the local Gradio URL shown in the terminal and sign in with Hugging Face
when prompted. The application uses the authenticated Hugging Face session for
Inference API requests; do not hard-code access tokens in source files or
notebooks.

## Development

Run the test suite with:

```powershell
python -m pytest
```

Generated virtual environments, caches, model files, and credentials should
remain untracked.
