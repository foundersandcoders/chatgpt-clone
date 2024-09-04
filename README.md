# ChatGPT Clone

This project is a reference implementation of a simple ChatGPT clone built using only front-end technologies: vanilla JavaScript and basic CSS.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [User stories](#user-stories)
- [Setup](#setup)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project aims to provide a basic understanding of how to create a simple chat application using vanilla JavaScript and CSS. It mimics the functionality of a chatbot where users can input text and receive predefined responses.

## Features

- Simple and clean user interface
- User input field for chat messages
- Display of user messages and bot responses
- Basic CSS styling for a pleasant user experience

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6)


## User stories

1. **Capture Form Data and Display on Page**: As a front-end developer, I want to start by writing a JavaScript function that captures the text from a textarea and displays it in a designated section on my web page when I press the submit button, using an **`onclick`** event handler and DOM manipulation methods like **`document.getElementById`** and **`textContent`**.
2. **API Key Entry**: As a front-end developer, I want to create a secure input field for entering my API key and storing it in a local variable, which I understand will only be for the learning process and not for a production environment.
3. **Store API Key Temporarily**: As a front-end developer, I want to temporarily store my entered API key in a JavaScript variable upon form submission and then remove the input field from the UI for subsequent chats.
4.  **Send API Requests**: As a front-end developer, I want to write a JavaScript function that sends the captured text to the OpenAI API, using the **`https://api.openai.com/v1/chat/completions`** endpoint with the API key in the header, and to get a response, using **`fetch()`** and **`.then()`** (and probably not using `async`/`await`, unless you are confident using it).
5. **Handle API Responses**: As a front-end developer, I want to take the response from the OpenAI API and display it in the designated section, using methods like **`JSON.parse()`** and **`JSON.stringify`** and updating the DOM to display the response.
6. **Enhance User Interaction**: As a front-end developer, I want to add CSS to make the interaction with my bot more visually appealing.

### Stretch stories

7. **Send Chat History with API Requests**: As a front-end developer, I want to include the chat history in each API request to OpenAI. This will involve appending previous chat messages and responses to the request payload, ensuring the AI can contextualise new messages based on the ongoing conversation.
8. **Create a separate config file for Environment Variables**: As a front-end developer, I aim to create my own config file for storing sensitive information like the OpenAI API key and exclude it from GitHub using a `.gitignore` file. I plan to manually load these variables at the start of my application, understanding this approach doesn't offer real security in a front-end only environment but is valuable for learning about environment variables.

## Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/foundersandcoders/chatgpt-clone.git
   ```
2. **Navigate to the project directory:**
   ```bash
   cd chatgpt-clone
   ```
3. **Open `index.html` in your web browser:**
   ```bash
   open index.html
   ```

## Usage

1. Open the `index.html` file in your web browser.
2. Type a message in the input field at the bottom of the chat window.
3. Press "Enter" or click the "Send" button to see the bot's response.

## Project Structure

```
chatgpt-clone/
├── index.html
├── styles.css
└── script.js
```

- `index.html`: The main HTML file that contains the structure of the chat application.
- `styles.css`: The CSS file that contains the styling for the chat application.
- `script.js`: The JavaScript file that contains the logic for handling user input and bot responses.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, please create a pull request or open an issue.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
