# EXP-9
# LLM JSON Output Generation and Validation

## Aim
To generate structured JSON output using an LLM and validate its syntax and schema.

## Problem Statement
Generate a JSON array containing exactly three books. Each book must have a title, author, and publication year.

## Technologies Used
- Python
- Groq API
- OpenAI Python SDK
- JSON

## Model
`llama-3.3-70b-versatile`

## Algorithm
1. Define a prompt requesting JSON-only output.
2. Send the prompt to the LLM.
3. Parse the response using `json.loads()`.
4. Validate the array length, keys, and value types.
5. If parsing or validation fails, retry once with a stricter prompt.
6. Print and save the validated JSON as `books.json`.

## Expected Output
A valid JSON array containing exactly three book objects with the keys `title`, `author`, and `year`.

## How to Run
Run the script in Google Colab after adding `GROQ_API_KEY` to Colab Secrets. Install dependencies with `pip install -r requirements.txt`.

## Security
Never upload API keys, credentials, or private environment files to GitHub.
