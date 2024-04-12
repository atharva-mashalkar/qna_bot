# Q and A Chat Bot

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Initializing the App](#initializing-the-app)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Introduction

The LLM Chat Bot is an intelligent application designed to enhance access to information within PDF documents. Users can upload multiple PDFs, from which the app extracts text and stores it in a FAISS vector store for efficient searching. The system allows users to pose questions related to the PDF content, which are then processed using OpenAI and Hugging Face APIs to provide relevant answers. This conversation is stored in-memory to utilize as context for future inquiries. This backend handles all core functionalities including PDF processing, data storage, API interactions, and dynamic context management.

## Getting Started

### Prerequisites

To run this application, you will need the following installed on your machine:

- Python (>=3.8)
- pip (Python package manager)

### Installation

Follow these steps to set up the project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/atharva-mashalkar/qna_bot.git
   cd qna_bot
   ```
   
2. Install the required Python packages:
  ```bash
    pip install -r requirements.txt
  ```

## Environment Variables

Before running the server, configure the necessary environment variables in a .env file in the root directory:

OPENAI_API_KEY: Your API key for OpenAI, used to fetch responses based on the document context.
HUGGINGFACE_API_KEY: Your API key for Hugging Face, which is used to utilize specific models for document processing and understanding.

## Initializing the App

To start the server and make the backend operational, use the following command:

```bash
streamlit run app.py
```

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated. If you have suggestions for improvements, please fork the repo and create a pull request or open an issue. Don't forget to give the project a star! Thanks again!

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

Thanks to the creators of the FAISS library for providing efficient similarity search algorithms.
Gratitude goes to the teams at OpenAI and Hugging Face for their incredible machine learning models and APIs.
Appreciation for Streamlit for making it easy to build and share beautiful custom web apps for machine learning and data science.
