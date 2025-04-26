# Gemini AI Chat Interface

A React-based chat interface for Google's Gemini AI model, providing a clean and intuitive way to interact with the powerful language model.

## Features

- **Modern UI** inspired by the official Gemini interface
- **Real-time AI responses** using Google's Generative AI API
- **Chat history** to track and revisit previous conversations
- **Expandable sidebar** for easy navigation
- **Suggestion cards** to help users get started

## Project Structure

```
src/
├── assets/
│   └── assets.js        # Central export for icons and images
├── components/
│   ├── Main/
│   │   ├── Main.jsx     # Main chat interface component
│   │   └── Main.css
│   └── Sidebar/
│       ├── Sidebar.jsx  # Sidebar navigation component
│       └── sidebar.css
├── config/
│   └── gemini.js        # Gemini API configuration
├── context/
│   └── Context.jsx      # React context for state management
└── App.jsx              # Root application component
```

## Setup and Installation

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Create a `.env` file in the root directory with your Gemini API key:
   ```
   REACT_APP_GEMINI_API_KEY=your_api_key_here
   ```
4. Start the development server:
   ```
   npm start
   ```

## API Configuration

This project uses the Google Generative AI JavaScript SDK to interact with the Gemini API. The configuration includes:

- Temperature: 0.9 (for creative responses)
- Safety settings to filter inappropriate content
- Support for multi-turn conversations

## Usage

1. Type your prompt in the input field at the bottom of the screen
2. Click the send icon or press Enter to submit
3. View the AI's response in the chat area
4. Access previous conversations from the sidebar

## Components

### Main

The central component displaying the chat interface, suggestion cards, and input field.

### Sidebar

Collapsible navigation panel showing chat history and application controls.

### Context Provider

Manages application state including:
- Current and previous prompts
- Loading states
- Chat results
- New chat initialization

## Dependencies

- React
- @google/generative-ai

## Security Note

Always protect your API keys and avoid exposing them in client-side code for production applications. Consider implementing a backend service to handle API calls securely.

## License

MIT

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/UmaMaheshkondaveti/Gemini-Clone
