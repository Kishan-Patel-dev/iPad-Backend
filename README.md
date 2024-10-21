# iPad Math Calculator Backend

This is the backend for the iPad Math Calculator project, built using Python with FastAPI. This backend handles requests from the frontend and performs necessary calculations.

## Table of Contents

- [Live Demo](#live-demo)
- [Demo Video](#demo-video)
- [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
- [File Structure](#file-structure)
- [Environment Variables](#environment-variables)
- [License](#license)

## Live Demo

You can try out the live demo of the iPad Math Calculator at the following link:

[Live Demo](https://calc-fe.vercel.app/)

## Demo Video

Check out the demo video showcasing the iPad Math Calculator functionality:
![Demo GIF](Project_demo_full.gif)


## Installation

To set up the project locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd ipad-be
   ```

2. Create a virtual environment:

   ```bash
   python3 -m venv venv
   ```

3. Activate the virtual environment:

   For Fish shell:

   ```bash
   source venv/bin/activate.fish
   ```

   For Bash or Zsh:

   ```bash
   source venv/bin/activate
   ```

4. Install the required packages:

   ```bash
   pip install fastapi Pillow uvicorn pydantic google.generativeai python-dotenv
   ```

5. Create a `.env` file in the root directory to store your environment variables. You can do this by running:

   ```bash
   touch .env
   ```

   Then, add your Gemini API key:

   ```plaintext
   # Gemini API Credentials
   GEMINI_API_KEY=your_api_key_here
   ```

   **Note:** The `.env` file is not included in the repository for security reasons. Make sure to add your credentials after creating the file.

## Usage

To run the application locally, execute the following command:

```bash
uvicorn app.calculator.route:app --reload
```

Visit `http://127.0.0.1:8000` in your browser to access the API.

## Development

During development, the following commands were used:

```bash
mkdir ipad-be
https://github.com/Kishan-Patel-dev/iPad-Backend.git
python3 -m venv venv
touch .env
pip install fastapi Pillow uvicorn pydantic google.generativeai python-dotenv
python3 main.py
```

## File Structure

```plaintext
ipad-be/
├── .gitignore
├── .env
├── .venv
├── __pycache__/
├── app/
│   └── calculator/
│       ├── __pycache__/
│       └── route.py
├── main.py
├── schema.py
└── constants.py
```

## Environment Variables

In the `.env` file, add your Gemini API credentials as follows:

```plaintext
# Gemini API Credentials
GEMINI_API_KEY=your_api_key_here
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
