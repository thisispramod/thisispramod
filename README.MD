# Hi there, I'm Pramod Kumar 👋

### 🚀 Senior Backend & Full-Stack Engineer | Golang & PHP Specialist
Building scalable backend microservices, high-performance REST APIs, and multi-tenant enterprise solutions. Experienced in cloud infrastructure, CI/CD pipelines, and database optimization.

⚡ **Status:** #OpenToWork — **Immediate Joiner** (0 Days Notice Period)

---

### 🛠️ Tech Stack

**Languages & Frameworks**

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Gin](https://img.shields.io/badge/Gin-00ADD8?style=flat-square&logo=go&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)

**Databases & Infra**

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-464B4E?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Core Architectural Concepts**  
`REST APIs` `gRPC` `JWT Authentication` `Goroutines & Channels` `CI/CD` `Role-Based Access Control (RBAC)`

---

### 📌 Featured Projects

#### 🎓 [SkillUp LMS — AI-Powered Learning Management System](https://github.com/thisispramod)
A microservices-based LMS built with **Go (Gin), React, MySQL, and Docker**. Features an AI-powered adaptive assessment engine (Groq/Llama 3.1), JWT-based role authorization, goroutine-driven concurrency, and a mastery-based learning engine with spaced repetition.  
`Go` `Gin` `React` `MySQL` `Docker` `REST APIs`

---

#### 📁 Smart Document Management Software — Enterprise Document Drive
A high-performance document repository and drive application built with microservices architecture.  
`Go` `PHP` `MySQL` `AWS S3` `REST APIs`

- Built Go microservices to handle large file uploads, versioning, and document metadata tracking.
- Integrated **AWS S3** for secure, scalable blob storage with pre-signed URLs for access control.
- Designed granular Role-Based Access Control (RBAC) for organization-wide file sharing permissions.
- Implemented streaming endpoints and chunked upload handling to optimize bandwidth and network performance.

---

#### 🔗 [BitURL – High-Performance URL Shortener Microservice](https://github.com/thisispramod/biturl)
[![Golang](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)](https://github.com/thisispramod/biturl)
[![GitHub](https://img.shields.io/badge/GitHub-thisispramod%2Fbiturl-181717?style=flat-square&logo=github)](https://github.com/thisispramod/biturl)

A lightweight, concurrent URL shortener service built using Go's standard `net/http` package. It generates deterministic 8-character hash identifiers for URLs using MD5 hashing and manages link redirection in memory.

**Key Highlights & Architecture:**
- **Standard Library HTTP Handlers:** Built using Go's standard `net/http` package for efficient request routing.
- **Deterministic Hash Generation:** Utilizes MD5 hashing (`crypto/md5`) sliced to 8 characters to produce unique short code IDs.
- **In-Memory Storage:** Fast key-value lookups using Go maps (`map[string]URL`) mapping unique IDs to URL structs with creation timestamps.
- **JSON API Responses:** Implemented JSON encoding and decoding (`encoding/json`) for structured API payload handling.

**Data Model:**
```go
type URL struct {
    ID           string    `json:"id"`
    OriginalURL  string    `json:"orginal_url"`
    ShortURL     string    `json:"short_url"`
    CreationDate time.Time `json:"creation_date"`
}
