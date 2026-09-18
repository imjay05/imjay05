<h1 align="center">Hi, I'm Jay !</h1>
<h3 align="center">Full-Stack Developer building Production-style Systems</h3>

<p align="center">
  <a href="https://github.com/imjay05"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/jay-shelke-4323a22a5/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" /></a>
  <a href="https://leetcode.com/u/imjay05/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=flat&logo=leetcode&logoColor=white" /></a>
  <a href="mailto:imjaydigambarshelke@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/Pune%2C%20India-000000?style=flat&logo=googlemaps&logoColor=white" />
</p>

---

### 🧑‍💻 About Me

- 🎓 B.E. in Information Technology, Rasiklal M. Dhariwal Sinhgad Technical Institutes Campus (SPPU) — Expected June 2027
- 🛠️ I build full-stack MERN systems that solve real engineering problems —  third-party API resilience
- 📫 Reach me at **imjaydigambarshelke@gmail.com**

---

### 🧰 Tech Stack

**Languages**
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

**Frontend**
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)

**Backend**
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=flat&logo=express&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white)

**Database**
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)

**Third-Party / AI Integrations**
![Gemini API](https://img.shields.io/badge/Gemini%20API-8E75B2?style=flat&logo=googlegemini&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat)
![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=flat&logo=cloudinary&logoColor=white)

---



### 🚀 Featured Projects

#### 🏥 HealthLense — AI-Powered Medical Report Analysis & Symptom Intelligence Platform
`Node.js` `Express` `React` `MongoDB` `Socket.io` `Groq` `Cloudinary`

Turns confusing medical reports into plain-language insights — in English, Hindi, or Marathi — and connects patients to nearby diagnostic labs in real time.

- **Cost-aware AI pipeline** — SHA-256 file hashing dedupes uploads before any Cloudinary/Groq call, cutting redundant inference and storage spend
- **Multi-modal document pipeline** — PDFs, DOCX, and images all funnel through a single vision-model path (PDFs converted to per-page JPEGs on the fly, capped at 4 pages)
- **Dependency-free rate limiting** — sliding-window limiter built on MongoDB TTL indexes (no Redis), with a deliberate fail-open policy so infra hiccups never block a real user
- **Resilient geocoding** — respects Nominatim's 1 req/sec limit with progressive radius expansion and name-based dedupe, streamed to the client over an authenticated Socket.IO channel

---

#### 📈 ArcTrade — Full-Stack Stock Trading Simulator
`React` `Node.js` `Express` `MongoDB` `Razorpay` `Yahoo Finance API`

**[Live Demo →](https://arctrade-stocks.vercel.app)**

A MERN trading platform simulating real-world investing — wallet funding via a real Razorpay checkout, a live watchlist of 50+ NSE stocks across 9 sectors, and a hand-built candlestick chart.

- **ACID-safe trading engine** — every order runs inside a MongoDB multi-document transaction; wallet debit, order creation, and holdings update all succeed or roll back together
- **Real weighted-average cost basis** — the same P&L logic real brokerages use, recalculated on every repeat buy
- **Verified payments** — server-side HMAC-SHA256 signature verification on every Razorpay payment before a single rupee is credited
- **Live-ish market data** — in-memory TTL cache with 8-wide batched parallel fetching, degrading gracefully to stale cached data (with a visible warning) if the upstream API fails

---
