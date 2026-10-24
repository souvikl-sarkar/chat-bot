# Chatbot Project

A small chatbot interface built with React and Vite. It displays a conversation, lets you type and send messages, and shows a chatbot reply using the `supersimpledev` package. The interface is split into reusable components for the message list, individual messages, and input area.

## Features

- Chat-style conversation with separate user and chatbot messages.
- Send a message with the **Send** button.
- Automatically scrolls the message area to the latest reply.
- Responsive styling for the chat interface.

## Requirements

- Node.js (npm is included with Node.js).
- A modern web browser.

## Run locally

Open a terminal in the project folder and install its dependencies:

```bash
npm install
```

Start the Vite development server:

```bash
npm run dev
```

Open the local address printed by Vite (usually [http://localhost:5173](http://localhost:5173)) in your browser. Keep the terminal running while you use the app. Press `Ctrl+C` in the terminal to stop the server.

## Use the chatbot

1. Type a message in the input at the bottom of the chat.
2. Click **Send**.
3. Your message and the chatbot's response appear in the conversation.

The chatbot response is provided by the `Chatbot` helper from `supersimpledev`. This demo does not connect to a custom server or require an API key. The conversation is held in React state, so it resets when the page is refreshed.

## Project structure

```text
.
├── index.html
├── src/
│   ├── App.jsx                    # App state and page composition
│   ├── App.css                    # App layout styles
│   ├── index.css                  # Global styles
│   └── components/
│       ├── ChatInput.jsx          # Message input and chatbot response
│       ├── ChatInput.css
│       ├── ChatMessages.jsx       # Conversation list and auto-scroll
│       ├── ChatMessages.css
│       ├── ChatMessage.jsx        # Individual message display
│       └── ChatMessage.css
├── package.json
└── vite.config.js
```

## Other commands

Run these from the project folder:

```bash
npm run build     # Build the production site into dist/
npm run preview   # Preview the production build locally
npm run lint      # Check the source with ESLint
```
