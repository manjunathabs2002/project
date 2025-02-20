# AI-Powered Code Reviewer

## Overview

The AI-Powered Code Reviewer is a tool designed to assist developers in reviewing and improving their code. It leverages the capabilities of Google's Generative AI to provide detailed feedback on code quality, best practices, performance, security, and more.

## Features

- **Code Quality**: Ensures clean, maintainable, and well-structured code.
- **Best Practices**: Suggests industry-standard coding practices.
- **Efficiency & Performance**: Identifies areas to optimize execution time and resource usage.
- **Error Detection**: Spots potential bugs, security risks, and logical flaws.
- **Scalability**: Advises on how to make code adaptable for future growth.
- **Readability & Maintainability**: Ensures that the code is easy to understand and modify.

## Setup

### Prerequisites

- Node.js (v20.15.1 or later)
- npm (Node Package Manager)
- A Google Generative AI API key

### Installation

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd AI_Powered Code Reviewer
    ```

2. Install the dependencies:
    ```sh
    cd Backend
    npm install
    ```

3. Create a `.env` file in the `Backend` directory and add your Google Generative AI API key:
    ```plaintext
    GOOGLE_GEMINI_KEY=your-google-gemini-api-key
    ```

## Usage

1. Start the backend server:
    ```sh
    npm start
    ```

2. The server will be running on `http://localhost:3000`.

3. Use the API to generate content by sending a POST request to `/generate` with a JSON body containing the `prompt`.

## Example

```sh
curl -X POST http://localhost:3000/generate -H "Content-Type: application/json" -d '{"prompt": "Review this code..."}'
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
