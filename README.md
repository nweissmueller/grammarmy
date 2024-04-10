Here's a README file for the provided code:

# Typo Correction with OLLAMA API

This Python script enables typo correction across all programs on a local macOS machine using the OLLAMA API. It provides keyboard shortcuts to fix the current line (F9) or selected text (F10) by sending the text to the OLLAMA API for correction.

## Features

- Fix typos, casing, and punctuation in the current line or selected text
- Preserve new line characters in the corrected text
- Seamless integration with any program on macOS

## Requirements

- macOS operating system
- Python 3.9+
- pynput
- pyperclip
- httpx
- OLLAMA (local installation)

## Installation

1. Ensure you have Python 3.9 or higher installed on your macOS machine.
2. Install the required Python packages:

   ```
   pip install pynput pyperclip httpx
   ```

3. Install OLLAMA locally and ensure it is running on `http://localhost:11434`.

## Usage

1. Run the script:

   ```
   python typo_correction.py
   ```

2. The script will start and listen for keyboard shortcuts.
3. To fix the current line, press `F9`. The script will automatically select the current line, send it to the OLLAMA API for correction, and replace the line with the corrected text.
4. To fix selected text, select the desired text and press `F10`. The script will copy the selected text, send it to the OLLAMA API for correction, and replace the selected text with the corrected text.
5. The corrected text will preserve any new line characters present in the original text.

## Configuration

- `OLLAMA_ENDPOINT`: The URL endpoint for the OLLAMA API. Default is `"http://localhost:11434/api/generate"`.
- `OLLAMA_CONFIG`: Configuration options for the OLLAMA API request. Default values are provided in the script.
- `PROMPT_TEMPLATE`: The prompt template used to format the text sent to the OLLAMA API for correction.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgments

- [OLLAMA](https://github.com/OLLAMA-ai/OLLAMA) - Open Large Language Model for Multilingual Applications
- [pynput](https://pypi.org/project/pynput/) - Python library for controlling and monitoring input devices
- [pyperclip](https://pypi.org/project/pyperclip/) - Python module for cross-platform clipboard support
- [httpx](https://www.python-httpx.org/) - Fast and easy-to-use HTTP client for Python

Feel free to customize and enhance this README file based on your specific needs and project details.
