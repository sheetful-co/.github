# 🚀 Welcome to Our Organization

We focus on building modern and scalable solutions using the latest tech stack. Our flagship project, **Sheetful**, reflects our commitment to quality and performance.

---

## 🛠️ Tech Stack & Tools

![Next JS](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-5433FF?style=for-the-badge&logo=stripe&logoColor=white)
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)

---

## 📊 Project Architecture

Below is a simplified flow of how our applications are structured, integrating authentication, payments, and external services.

```mermaid
graph TD
    User[👤 User] -->|Accesses| Client[🖥️ Frontend (Next.js)]
    Client -->|API Requests| API[⚙️ API Routes]
    
    subgraph Backend Services
        API -->|Auth & Data| Supabase[(🗄️ Supabase)]
        API -->|Payments| Stripe[💳 Stripe]
        API -->|Emails| Resend[📧 Resend]
        API -->|Integration| Google[📑 Google APIs]
    end
    
    subgraph Deploy
        Client -.-> Vercel[☁️ Vercel]
    end
    
    classDef primary fill:#2563eb,stroke:#1d4ed8,color:white;
    classDef secondary fill:#475569,stroke:#334155,color:white;
    classDef database fill:#059669,stroke:#047857,color:white;
    
    class User,Client primary;
    class API,Stripe,Resend,Google secondary;
    class Supabase database;
```

---

## 🌟 Featured Projects

### Premium SaaS Starter (Sheetful)
A complete SaaS platform, including:
- **Authentication** via Supabase
- **Payments** via Stripe
- **Integrations** with Google APIs
- **Landing Page** optimized for conversion

---

## 📫 Contact

Feel free to explore our repositories and contribute!

[![Website](https://img.shields.io/badge/Website-sheetful.co-blue?style=flat-square&logo=google-chrome)](https://sheetful.co)
