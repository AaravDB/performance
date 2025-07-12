# Performance 🎯

A high-performance **FastAPI** backend showcasing efficient response times, deployed on Render.

## 🚀 Project Overview

This project provides a simple yet powerful HTTP API built with **FastAPI**, designed for speed and low latency. It offers endpoints for:

- Basic health check (`/health`)
- A dynamic "ping-pong" service with processing time reporting (`/ping?q=`)
- Simulated heavy workload via delay (`/delay/{seconds}`)

You can explore the live API here: https://performance-2vof.onrender.com

## 🛠️ Tech Stack & Tools

- **FastAPI** – Fast, intuitive, and efficient web framework :contentReference[oaicite:1]{index=1}  
- **Uvicorn** – ASGI server optimized for asynchronous performance  
- **Python 3.10+** – Leverages type hints for robustness and editor support  
- **Render** – Free deployment platform for web services :contentReference[oaicite:2]{index=2}

## 📦 Setup & Run Locally

1. Clone the repo:  
   ```bash
   git clone https://github.com/AaravDB/performance.git
   cd performance
Create a virtual environment & install dependencies:

bash
Copy
Edit
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
Run the server:

bash
Copy
Edit
uvicorn main:app --reload
Visit http://127.0.0.1:8000/docs for interactive API docs (Swagger UI).

🧪 API Endpoints
GET /health
✅ Returns {"status": "ok"} if server is running

GET /ping?q=<message>
↔️ Returns the original message and measured latency

GET /delay/{seconds}
⏱️ Simulates a long-running task by pausing for the specified seconds

🌐 Deployment
Automatically deployed to Render.
Uses a free-tier web service with auto-sleep after inactivity (< 15 minutes) 
GitHub
.

🛠️ Why "Performance"?
This application is a lightweight testbed to:

Showcase FastAPI's low-latency response capabilities

Demonstrate FastAPI + Uvicorn performance in real-world scenarios

Serve as a template for deploying fast APIs with minimal setup

📈 Next Steps
Integrate benchmarking (e.g. using Locust or wrk)

Add caching or rate limiting

Introduce authentication for secure endpoints

Containerize via Docker for more flexible deployment

Feel free to tweak any section to better match your vision. Let me know if you'd like additional badges, screenshots, or examples!











Sources

Ask ChatGPT


  
