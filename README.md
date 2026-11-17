# 200-OK-Distributed-Chat

## Simple Distributed Chat Website

A lightweight, two-node distributed chat application built using Python, WebSockets, HTML, CSS, and JavaScript. This project demonstrates distributed systems concepts such as inter-server communication, message synchronization, user presence, concurrency, and basic fault tolerance.

## Contributors
- Moriah Lane
- Emmanuel Nsiah
- Drake Madesian
- Suraj Shrestha

## Project Overview

This project allows users to communicate in real time through two independent Python chat servers. Users can connect to either server and exchange messages with users connected to both servers.

The two servers communicate using WebSockets to synchronize online users and forward messages between nodes.

## Objectives
- Build a real-time web-based chat application.
- Implement two independent Python chat servers.
- Enable communication between the two servers.
- Track online users and their connected servers.
- Support message delivery between different servers.
- Maintain message ordering.
- Demonstrate basic fault tolerance through server reconnection.

## System Architecture

The application consists of:
- **Server 1:** Handles users connected to the first server.
- **Server 2:** Handles users connected to the second server.
- **Frontend:** Provides the chat interface using HTML, CSS, and JavaScript.
- **WebSockets:** Enable real-time communication between clients and servers and between the two servers.

If one server becomes unavailable, users can reconnect to the remaining server.

## Technologies Used

- Python
- WebSockets
- HTML
- CSS
- JavaScript
- TCP/IP
- Visual Studio Code
- GitHub

## Project Structure

```text
200-OK-distributed-chat/
│
├── server1.py
├── server2.py
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── requirements.txt
└── README.md
```

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/200-OK-distributed-chat.git
```

2. Navigate to the project folder:

```bash
cd 200-OK-distributed-chat
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Start Server 1:

```bash
python server1.py
```

5. Open another terminal and start Server 2:

```bash
python server2.py
```

6. Open the frontend in a web browser and connect users to either server.

## Expected Results

- Multiple users can connect simultaneously.
- Users on different servers can exchange messages.
- Online users and their server connections are tracked.
- Messages are delivered in the intended order.
- Users can reconnect if one server becomes unavailable.

## Distributed Systems Concepts

This project demonstrates:
- Distributed architecture
- Inter-server communication
- Concurrency
- State synchronization
- Message ordering
- Basic fault tolerance

## Limitations

The application focuses on basic text messaging and does not include video calls, voice calls, file sharing, complex authentication, or advanced user profiles.

---

**Team 200 OK | Simple Distributed Chat Website**
