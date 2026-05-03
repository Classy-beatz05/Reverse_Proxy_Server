# ORCHATHON — Next-Gen Reverse Proxy & API Gateway

A production-ready Reverse Proxy Server built with Node.js that protects backend applications using:

✅ Web Application Firewall (WAF)  
✅ Rate Limiting  
✅ Circuit Breaker Pattern  
✅ IP Blacklisting  
✅ Health Checks  
✅ Request Tracing  
✅ Real-time Security Dashboard  
✅ Structured JSON Logging  

---

## Architecture

Client → Reverse Proxy → Backend Server

Security Pipeline:

Client Request  
↓  
IP Blacklist Check  
↓  
WAF Inspection (SQLi / XSS / Path Traversal / Command Injection)  
↓  
Rate Limiting  
↓  
Circuit Breaker Validation  
↓  
Forward Request to Backend  

---

## Features

### Web Application Firewall (WAF)
Detects and blocks:

- SQL Injection
- XSS Attacks
- Path Traversal
- Command Injection

---

### Rate Limiter
Sliding window log implementation:

- Per IP
- Per endpoint
- Configurable rules

---

### Circuit Breaker
Prevents backend overload:

- CLOSED → normal traffic
- OPEN → blocks requests
- HALF_OPEN → recovery mode

---

### Real-time Dashboard
Monitor:

- Total Requests
- Blocked Requests
- Request Rate
- Avg Latency
- Security Events
- Top Attackers
- Live Logs

---

## Tech Stack

- Node.js
- HTTP / HTTPS
- JSON Config Engine
- SSE Dashboard
- Custom Middleware Logic

---

## Deployment

Hosted on Render.

Backend:
https://orchathon-backend.onrender.com

Proxy:
https://orchathon-proxy.onrender.com

---

## Future Enhancements

- JWT Authentication
- Redis-based distributed rate limiting
- Kubernetes deployment
- AI-based anomaly detection
- Geo-blocking
- API analytics

---

## Team ORCHATHON
Hackathon Project 🚀
