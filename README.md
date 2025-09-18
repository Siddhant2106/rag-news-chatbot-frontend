# RAG News Chatbot Frontend

This is the frontend for the **RAG News Chatbot** application. It provides a chat interface where users can ask questions about recent news, and receive AI-generated answers with relevant news sources. The frontend is built with React and communicates with a backend server via REST API and WebSockets.

---

## Features

- **Chat with AI:** Ask questions about the latest news and get summarized answers.
- **Source Attribution:** Each answer includes links to the news articles used.
- **Session Management:** Start new chat sessions and clear previous conversations.
- **Real-time Updates:** Uses WebSockets for instant message delivery.

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- [npm](https://www.npmjs.com/)

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/Siddhant2106/rag-news-chatbot-frontend.git
   cd rag-news-chatbot-frontend
   ```

2. **Install dependencies:**
   ```sh
   npm install
   ```

3. **Configure the backend URL (optional):**
   - By default, the app connects to the backend at:
     - `http://localhost:5000/api` (development)
     - `https://rag-chatbot-backend-xs79.onrender.com/api` (production)
   - To change this, edit `src/services/api.js` and `src/services/socket.js`.

---

### Running the Application

#### Development Mode

```sh
npm start
```
- Opens the app at [http://localhost:3000](http://localhost:3000).
- The page reloads automatically on code changes.

#### Production Build

```sh
npm run build
```
- Builds the app for production to the `build` folder.

---

## Usage

1. **Start the backend server** (see backend README for instructions).
2. **Start the frontend** using `npm start`.
3. Open your browser to [http://localhost:3000](http://localhost:3000).
4. Type your news-related question in the chat box and press send.
5. The chatbot will respond with a summary and links to relevant news articles.

---

## Project Structure

- `src/pages/ChatPage.js` — Main chat interface.
- `src/services/api.js` — Handles REST API calls.
- `src/services/socket.js` — Handles WebSocket connections.
- `src/components/` — UI components.

---

## Troubleshooting

- **API errors:** Ensure the backend server is running and accessible.
- **WebSocket issues:** Check that the backend supports socket connections and CORS is configured.
- **Dependency errors:** Run `npm install` to ensure all packages are installed.

---

## License

This project is for educational/demo purposes.

---

## Learn More

-