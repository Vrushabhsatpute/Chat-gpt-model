# SigmaGPT / Chat-GPT-Model

A full-stack AI chat application that communicates with a Large Language Model (LLM) using an API key to generate responses. The platform allows users to create chat threads and interact with an AI assistant in real time.

---

## 🚀 Features

* AI powered chat interface
* Thread-based conversation storage
* Backend API for LLM communication
* MongoDB database for storing chat history
* REST API architecture
* Modular backend structure
* Separate frontend and backend layers

---

## 🏗️ Project Structure

```
SigmaGPT-main
│
├── Backend
│   ├── models
│   │   └── Thread.js
│   ├── routes
│   │   └── chat.js
│   ├── utils
│   │   └── openai.js
│   ├── server.js
│   ├── package.json
│
├── Frontend
│
├── .gitignore
└── README.md
```

---

## ⚙️ Tech Stack

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose

### AI Integration

* OpenAI / LLM API

### Frontend

* JavaScript
* React (or any UI framework used)

---

## 📦 Installation

Clone the repository

```bash
git clone https://github.com/Vrushabhsatpute/Chat-gpt-model.git
```

Navigate to project folder

```bash
cd SigmaGPT-main
```

Install backend dependencies

```bash
cd Backend
npm install
```

---

## 🔑 Environment Variables

Create a `.env` file inside the backend folder.

Example:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
OPENAI_API_KEY=your_api_key
```

---

## ▶️ Running the Project

Start the backend server

```bash
npm start
```

Or using nodemon

```bash
npm run dev
```

Server will start on:

```
http://localhost:5000
```

---

## 🧠 API Flow

1. User sends message from frontend
2. Backend receives request
3. Message is sent to LLM API
4. AI response is returned
5. Conversation is stored in MongoDB thread

---

## 📡 Example API Endpoint

```
POST /api/chat
```

Request Body

```json
{
  "message": "Hello AI"
}
```

Response

```json
{
  "response": "Hello! How can I help you today?"
}
```

---

## 🗂️ Database Schema

### Thread Schema

Stores conversations with roles:

* user
* assistant

Each message includes:

* role
* content
* timestamp

---

## 🔮 Future Improvements

* Authentication system
* Streaming responses
* Chat history UI
* Multiple AI models
* User sessions

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Submit a pull request

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

Vrushabh Satpute

GitHub
https://github.com/Vrushabhsatpute
