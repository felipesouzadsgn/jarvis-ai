# J.A.R.V.I.S. - AI Chat Agent

J.A.R.V.I.S. (Just A Rather Very Intelligent System) is a single-page web application that provides an AI-powered chat interface. It leverages Google's Gemini API for language model capabilities and Firebase for conversation persistence.

## Key Features

- **AI-Powered Chat:** Utilizes Google's Gemini API for intelligent conversation.
- **Markdown Rendering:** AI responses are rendered with Markdown for rich text formatting (headings, lists, code blocks, etc.).
- **Conversation History:**
    - Chat history is stored and retrieved from Firestore.
    - A toggleable sidebar displays the list of past conversations.
- **Message Summarization:** Option to summarize the current conversation.
- **Message Translation:** AI messages can be translated into English.
- **Export to Markdown:** Current conversation can be exported as a Markdown file.
- **New Conversation:** Easily start a new chat session.
- **Animated Background:** Features a dynamic, animated gradient mesh background ("Nebula Flow" theme).
- **Minimalist UI:** Employs icon-only buttons (using Phosphor Icons) for a clean and modern interface.
- **Responsive Design:** Adapts to different screen sizes, including a mobile-friendly sidebar.

## Running the Project

J.A.R.V.I.S. is a static web application built with HTML, CSS, and vanilla JavaScript.

1.  **Open `index.html`:** Simply open the `index.html` file in a modern web browser.
2.  **Firebase Configuration (Required for Full Functionality):**
    *   To enable conversation history and persistence, you need to set up a Firebase project.
    *   The application expects Firebase configuration variables (`__firebase_config`) and an initial authentication token (`__initial_auth_token`) to be available in the global scope when `index.html` loads. These are typically injected or defined in a script before the main application script.
    *   You will also need to configure Firestore rules for your database.
3.  **Gemini API Key (Required):**
    *   The chat functionality relies on Google's Gemini API.
    *   You need to obtain an API key from Google AI Studio.
    *   Replace the placeholder `AIzaSyDVCKKMJPOUfCEAImb7weVojJcta22WLnY` for the `API_KEY` constant within the `<script type="module">` tag in `index.html` with your actual Gemini API key.

**Note:** Without valid Firebase and Gemini API configurations, the chat history and AI functionalities will not work correctly. The application may show warnings or errors in the browser console.

## Visual Style

-   **Theme:** The application uses a custom "Nebula Flow" theme, characterized by a dark base, animated vibrant gradient backgrounds, and cyan/blue accents for interactive elements.
-   **Inspiration:** The clean component design is inspired by ShadCN/UI.
-   **Icons:** Phosphor Icons are used for a consistent and minimalist icon set.

## Developed By

J.A.R.V.I.S. was created and developed by Felipe Souza.

## Features

*   **Real-time AI Chat:** Engage in natural conversations with an AI assistant.
*   **Conversation History:** Past conversations are saved and can be revisited.
*   **User Authentication:** Secure user login and registration.
*   **Responsive Design:** Adapts to different screen sizes for a seamless experience on desktop and mobile devices.

## Tech Stack

*   **Frontend:** HTML, CSS, JavaScript
*   **Language Model:** Google Gemini API
*   **Backend (for conversation persistence):** Firebase

## Getting Started

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/jarvis-chat-agent.git
    ```
2.  **Set up Firebase:**
    *   Create a Firebase project at [https://console.firebase.google.com/](https://console.firebase.google.com/).
    *   Obtain your Firebase project configuration (apiKey, authDomain, projectId, etc.).
    *   Replace the placeholder Firebase configuration in `script.js` with your actual project configuration.
3.  **Set up Google Gemini API:**
    *   Obtain an API key from [https://makersuite.google.com/](https://makersuite.google.com/).
    *   Replace the placeholder API key in `script.js` with your actual API key.
4.  **Open `index.html` in your browser.**

## Usage

*   Sign up for a new account or log in if you already have one.
*   Type your messages in the chat input field and press Enter to send.
*   The AI's responses will appear in the chat window.
*   You can view your past conversations in the conversation history panel.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any bugs or feature requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
