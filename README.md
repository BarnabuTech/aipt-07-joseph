# 🚀 Prompt-Powered Kickstart: Getting Started with Go (Golang)

## 📌 Project Objective

This project is a **beginner-friendly toolkit** designed to help new developers quickly get started with **Go (Golang)** using the support of **Generative AI prompts**. The goal is to demonstrate how AI can accelerate learning, setup, debugging, and documentation when exploring a new programming language.

The end result is a **minimal, runnable Go HTTP server** that responds with a simple message, serving as a foundation for backend and API development.

---

## 🧠 Why Go (Golang)?

Go is a modern, open-source programming language developed by Google. It is known for its simplicity, performance, and strong support for concurrency.

### Where Go Is Used

- Backend web services and APIs
- Cloud-native applications
- Microservices architectures
- Developer tools (e.g., Docker, Kubernetes)

### Real-World Example

Many large-scale systems such as **Kubernetes**, **Docker**, and **Terraform** are written in Go, making it a valuable language for backend and cloud engineers.

---

## 🖥️ System Requirements

To run this project, you need:

- **Operating System:** Linux, macOS, or Windows
- **Go Version:** Go 1.20 or higher
- **Editor (Recommended):** VS Code
- **Terminal Access**

Verify Go installation:

\`\`\`bash
go version
\`\`\`

---

## ⚙️ Installation & Setup Instructions

### Step 1: Install Go

Download and install Go from the official website:

👉 [https://go.dev/dl/](https://go.dev/dl/)

### Step 2: Clone the Repository

\`\`\`bash
git clone <https://github.com/BarnabuTech/aipt-07-joseph.git>
cd main.go
\`\`\`

### Step 3: Run the Application

\`\`\`bash
go run main.go
\`\`\`

---

## ✅ Minimal Working Example

### 📄 main.go

\`\`\`go
package main

import (
    "fmt"
    "net/http"
)

// helloHandler handles incoming HTTP requests
func helloHandler(w http.ResponseWriter, r *http.Request) {
    fmt.Fprintln(w, "Hello, welcome to Go with GenAI!")
}

func main() {
    // Register route
    http.HandleFunc("/", helloHandler)

    fmt.Println("Server running on http://localhost:8080")

    // Start HTTP server
    http.ListenAndServe(":8080", nil)
}
\`\`\`

---

## 🔍 What This Example Does

- Creates a basic HTTP server using Go's standard library
- Listens on port 8080
- Responds with a message when accessed via a browser

---

## 🌐 Expected Output

Open your browser and visit:

\`\`\`
<http://localhost:8080>
\`\`\`

**Output:**

\`\`\`
Hello, welcome to Go with GenAI!
\`\`\`

---

## 🤖 AI Prompt Journal & Learning Reflection

### Prompt 1

**Prompt Used:**

> "Give me a step-by-step guide to build a simple Hello World API in Go."

**How It Helped:**

The AI provided a clear explanation of Go's `net/http` package and how to structure a minimal server without external frameworks.

---

### Prompt 2

**Prompt Used:**

> "Explain this Go HTTP server code line by line for a beginner."

**How It Helped:**

This prompt helped me understand handler functions, routing, and how Go manages HTTP requests and responses internally.

---

### Prompt 3

**Prompt Used:**

> "What common errors do beginners face when running Go servers and how can they fix them?"

**How It Helped:**

The AI helped identify issues such as port conflicts, missing Go installations, and PATH configuration problems.

---

## ✨ Reflection

Using Generative AI significantly improved my learning speed and confidence. Instead of searching through multiple tutorials, I was able to:

- Learn Go fundamentals faster
- Debug errors efficiently
- Write clearer documentation
- Focus on understanding concepts instead of setup struggles

---

## ⚠️ Common Issues & Fixes

### Issue 1: `go: command not found`

**Cause:** Go is not installed or not added to PATH

**Fix:** Reinstall Go and ensure `$GOPATH/bin` is added to PATH

---

### Issue 2: `listen tcp :8080: bind: address already in use`

**Cause:** Port 8080 is already in use

**Fix:** Stop the conflicting process or change the port number

---

### Issue 3: Browser shows no response

**Cause:** Server not running

**Fix:** Ensure `go run main.go` is running successfully in the terminal

---

## 🧪 Testing & Iteration

This project was tested by:

- Running the server locally
- Accessing the endpoint via browser
- Reviewing the documentation clarity with a peer
- Iterating on explanations based on feedback

---

## 📚 References

- [Go Official Documentation](https://go.dev/doc/)
- [Go net/http Package](https://pkg.go.dev/net/http)
- [Moringa AI Learning Platform](https://ai.moringaschool.com)
- [Go Tour (Interactive)](https://tour.golang.org/)
