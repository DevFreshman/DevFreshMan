<!-- Profile README - DevFreshMan -->

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1100&color=6EE7F7&center=true&vCenter=true&width=820&lines=Hi%2C+I%27m+Ho%C3%A0ng+%C4%90%E1%BB%A9c+M%E1%BA%A1nh+%F0%9F%91%8B;Backend+Developer+%E2%80%94+Java+%26+Spring+Boot;Business+Logic+%26+Clean+Architecture;Building+systems+that+stay+easy+to+change" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/hoangducmanh/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-hoangducmanh-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  &nbsp;
  <a href="https://web.facebook.com/hoang.uc.manh.466145/" target="_blank">
    <img src="https://img.shields.io/badge/Facebook-Profile-1877F2?style=for-the-badge&logo=facebook&logoColor=white" />
  </a>
  &nbsp;
  <a href="https://github.com/DevFreshMan" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-DevFreshMan-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=DevFreshMan&style=flat-square&color=6EE7F7&label=Profile+Views" />
</p>

<br/>

---

## About

I build backend services with **Java / Spring Boot**, focusing on **clear business logic** and **clean boundaries**.  
I care about systems that remain **easy to evolve** as requirements change.

**Current interests**

- Clean Architecture / Hexagonal (Ports & Adapters)
- Use-case driven service design
- Database design & performance (**MySQL + PostgreSQL**)

---

## Tech

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,docker,git,github,postgres,mysql,redis&theme=dark" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Boot_3+-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL_15-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL_8-4479A1?style=flat-square&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker_Compose-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Swagger_OpenAPI-85EA2D?style=flat-square&logo=swagger&logoColor=black" />
</p>

---

## Featured Projects

### 📋 Smart Task Management System — Hexagonal Architecture

A RESTful backend API for personal/team task management, built with **Hexagonal Architecture (Ports & Adapters)** — the **domain layer stays pure Java** (no Spring/JPA dependencies).

<p>
  <img src="https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker_Compose-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black" />
</p>

**Key features**
- JWT Authentication: **Access token (15m)** + **Refresh token (7d)** with revoke
- Task CRUD with **soft-delete**
- Task status **state machine**: `TODO → IN_PROGRESS → COMPLETED` (no skipping)
- Role-based access: **USER / ADMIN**
- Filtering + sorting + pagination (status/priority/deadline)
- Redis cache with `@Cacheable` / `@CacheEvict`
- Rate limiting: **max 5 failed logins / 15 min / IP**
- Audit log via **Spring AOP** (create/update/delete)
- Deadline reminder scheduler (daily **8:00 AM**)
- Comments with permission checks (author or ADMIN)

[![View Repository](https://img.shields.io/badge/View_Repository-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/DevFreshman/Smart-Task-Management)

### 🌱 Seed Entry E-commerce Platform — Full-stack

A full-stack e-commerce web app for buying/selling **plant seedlings**, built as a **monolithic three-tier architecture**:
**React (UI) → Spring Boot (Business) → MySQL (Data)**.

<p>
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL_8-4479A1?style=flat-square&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Google_OAuth-4285F4?style=flat-square&logo=google&logoColor=white" />
</p>

**Key features**
- Authentication: Register/Login (JWT), **Google OAuth**, refresh token, logout
- Product browsing, search & filter (category/type), product details
- Shopping cart: add/update/remove/clear
- Order processing: create order from cart, store OrderItems + Transaction
- Send **order confirmation email**
- User profile management + transaction history (filter by status)

[![View Repository](https://img.shields.io/badge/View_Repository-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/DevFreshman/E-Commerce-Web)

## How I approach architecture (practical)

- Keep **business rules** independent from frameworks as much as possible
- Prefer **explicit use cases** (clear flows, easier testing)
- Isolate infrastructure behind interfaces / adapters (DB / cache / external services)
- Optimize for **readability and change** — not cleverness

---

## GitHub

<p align="center">
  <img src="https://streak-stats.demolab.com?user=DevFreshMan&theme=tokyonight&hide_border=true&border_radius=12" />
</p>


---
