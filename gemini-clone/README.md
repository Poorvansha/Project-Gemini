# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
- 
Project Name: Gemini - Conversational AI Web Application
Overview
Gemini is a web-based application that integrates Google Generative AI (specifically the Gemini 1.5 model) to provide an interactive conversational experience. The application features a user-friendly interface, enabling users to interact with AI through various prompts and receive responses in a dynamic and visually appealing format.

Project Structure
components

Main: Contains the main content of the application, including greeting the user, displaying suggestion cards, and showing the result of the user's prompt.
Sidebar: Contains navigation elements, recent chats, and options for initiating new conversations or accessing settings.
context

Context.js: Provides a context API setup for managing the global state of the application, including user input, recent prompts, loading state, and the AI-generated responses.
config

gemini.js: Contains the configuration for integrating with Google's Generative AI (Gemini model) and the logic for processing and sending prompts to the AI model.
assets

Contains various icons used throughout the UI, such as menu, history, setting, and more.
App.js

The root component that combines the Sidebar and Main components to form the application's main interface.
index.css

The main stylesheet that imports Google Fonts and applies global styles, animations, and layout settings for the entire application.
Key Features
User Interface:

Clean and modern UI design using CSS and React.
Sidebar with recent prompts, new chat functionality, and additional options like Help and Settings.
Main content area with dynamic greeting, suggestion cards, and display of AI-generated responses.
Conversational AI Integration:

Integration with Google Generative AI (Gemini 1.5) to process user prompts.
Safety settings to filter out harmful content such as hate speech, harassment, sexually explicit content, and dangerous content.
Response handling to format and display the output in a user-friendly format, including the use of bold text and line breaks.
State Management:

Utilizes React Context API to manage the application's global state, including handling user input, loading states, and storing previous prompts.
Installation
Prerequisites
Node.js and npm should be installed on your machine.
Setup Instructions
Clone the Repository:

bash
Copy code
git clone https://github.com/your-username/gemini-conversational-ai.git
cd gemini-conversational-ai
Install Dependencies:

bash
Copy code
npm install
Setup Environment Variables:

Replace the API key in the gemini.js file with your own Google Generative AI API key.
Run the Application:

bash
Copy code
npm start
The application will start on http://localhost:3000.
Usage
Starting a Conversation:
Enter a prompt in the search box at the bottom of the main section and hit the send icon to receive a response from the AI.
Navigating the Interface:
Use the Sidebar to access recent prompts, start a new chat, or adjust settings.
Viewing Results:
The response from the AI will be displayed in the result area with formatting enhancements for readability.
Customization
Icons and Assets:

Icons can be replaced or modified by adding new assets in the assets folder and updating the imports and assets object accordingly.
Styling:

Modify the styles in index.css, Main.css, and Sidebar.css to change the look and feel of the application.
AI Configuration:

Adjust the temperature, topP, topK, and other parameters in the gemini.js file to tweak the behavior of the AI model.
