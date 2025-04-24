# CisCall


CisCall is a Cisco-themed, accountless video conferencing and live-streaming platform built with Go, Fiber and Pion/WebRTC.

![CisCall Demo](./demogif.gif)

---

## 🚀 Features

- **Cisco-Inspired UI** — Clean, modern design with familiar Cisco “bridge bars” motif  
- **Join Without Accounts** — No sign-ups, no passwords, just click and talk  
- **Browser-Only** — Zero installs; works on desktop & mobile  
- **Free & Open-Source** — MIT-licensed, forever free  
- **Live Streaming** — Broadcast your meetings publicly via stream links  
- **Self-Hostable** — Deploy on your own servers or Fly.io with the provided configs  
- **Real-Time Chat** — Text chat alongside video in every room  
- **Viewer Mode** — Let participants join in “view-only” mode  

---

## 💻 Tech Stack

- **Go 1.19+** — Backend language  
- **Fiber v2** — High-performance web framework  
- **Pion WebRTC** — Real-time audio/video engine  
- **FastHTTP WebSocket** — Low-latency WebSocket support  
- **Fiber Template (HTML)** — Server-side HTML templates  
- **Static Assets** — CSS, JS, icons in `assets/`  

---

## 🏁 Getting Started

### Prerequisites

- Go 1.19 or newer  
- Git

### Installation

```bash
# Clone the repo
git clone https://github.com/harriputterr/ciscall.git

# Build the CLI/server
cd ciscall/cmd
go build -o ciscall
```

### Configuration

- **PORT** (env var) — Port to listen on (default `8080`)  
- **TLS** — Pass `-cert /path/to/cert.pem -key /path/to/key.pem` flags to enable HTTPS  

### Run

```bash
# Local HTTP
./ciscall -addr :8080

# Or HTTPS
./ciscall -addr :443 -cert server.crt -key server.key
```

Open your browser at `http://localhost:8080` (or `https://…`).

---

## 📂 Project Structure

```
ciscall/
├── cmd/               # Entrypoint (main.go)
├── internal/
│   ├── handlers/      # HTTP route handlers
│   └── server/        # Server setup & middleware
├── pkg/
│   └── webrtc/        # Room & peer management
├── assets/            # Static CSS, JS, fonts, icons
├── views/             # HTML templates
├── doc/               # Preview GIF & documentation images
├── Dockerfile         # Container build instructions
├── fly.toml           # Fly.io deployment config
├── go.mod             # Go module file
└── go.sum             # Go dependencies lockfile
```  

---

## 🤝 Contributing

Contributions are very welcome!   

1. Fork the repo  
2. Create a feature branch (`git checkout -b feature/my-cool-feature`)  
3. Commit your changes (`git commit -m "Add awesome feature"`)  
4. Push and open a Pull Request  

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 👤 Author

**Harsingh Sekhon**  
LinkedIn: [harsingh-sekhon](https://www.linkedin.com/in/harsingh-sekhon/)

