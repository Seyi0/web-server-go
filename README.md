# Web Server in Go 🌐

This repository contains a simple web server written in Go. It demonstrates basic routing, handling different HTTP methods, and serving static files.

---

## Features ✨
- **Static File Serving**: Serves `index.html` from the `./static` directory.  
- **Form Handling**: Processes `POST` requests sent to the `/form` endpoint and extracts form data.  
- **Basic API Endpoint**: Responds to `GET` requests at the `/hello` endpoint with a simple `"hello!"` message.  
- **Error Handling**: Provides appropriate error messages for unsupported HTTP methods and non-existent routes.  

---

## Endpoints 🚀

### `GET /`
- Serves the `index.html` file located in the `static` directory.  
- This is the root endpoint of the web application.  

### `GET /hello`
- Responds with the text `"hello!"`.  
- Only `GET` requests are supported; any other method will return a **404 not found** error.  

### `POST /form`
- Handles form submissions.  
- Expects `POST` requests with form data containing **name** and **address** fields.  
- The server prints the submitted name and address to the console.  

---

## Getting Started 🏃‍♂️

### Prerequisites
- [Go](https://go.dev/dl/) (version **1.16** or higher) must be installed on your system.  

### Running the Server
1. Clone this repository or save the provided code to a `.go` file (e.g., `main.go`).  
2. Create a folder named `static` in the same directory as the Go file.  
3. Inside the `static` folder, create an `index.html` file.  
4. Run the application from your terminal:  

   ```bash
   go run main.go
### Project Structure 📁
.
├── main.go               # The main Go application file
└── static/
    └── index.html        # The static HTML file served by the server

