<div align="center">
  <a href="https://sheetful.co">
    <img src="https://sheetful.co/logotipo.svg" alt="Sheetful Logo" width="120" />
  </a>
  <h1>Welcome to Sheetful</h1>
  <p>
    <a href="https://app.sheetful.co">
      <img src="https://img.shields.io/badge/GET%20STARTED-16B364?style=for-the-badge&logo=rocket&logoColor=white" alt="Get Started" />
    </a>
    &nbsp;
    <a href="https://sheetful.co/docs">
      <img src="https://img.shields.io/badge/DOCUMENTATION-16B364?style=for-the-badge&logo=googledocs&logoColor=white" alt="Documentation" />
    </a>
  </p>
</div>

We focus on building modern and scalable solutions using the latest tech stack. Our flagship project, **Sheetful**, reflects our commitment to quality and performance.

---

## Tech Stack & Tools

![Next JS](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-5433FF?style=for-the-badge&logo=stripe&logoColor=white)
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)

---

## Project Architecture

Below is a simplified flow of how our applications are structured, integrating authentication, payments, and external services.

```mermaid
graph LR
    User["User"] -->|Accesses| Client["Frontend (Next.js)"]
    
    subgraph "Next.js App"
        Client -->|Requests| API["API Routes"]
    end
    
    subgraph "Infrastructure"
        Client -.->|Deployed on| Vercel["Vercel"]
    end
    
    subgraph "External Services"
        direction TB
        Supabase[("Supabase")]
        Stripe["Stripe"]
        Resend["Resend"]
        Google["Google APIs"]
    end
    
    API -->|Auth & Data| Supabase
    API -->|Payments| Stripe
    API -->|Emails| Resend
    API -->|Integrations| Google
    
    classDef primary fill:#2563eb,stroke:#1d4ed8,color:white;
    classDef secondary fill:#475569,stroke:#334155,color:white;
    classDef database fill:#059669,stroke:#047857,color:white;
    
    class User,Client primary;
    class API,Stripe,Resend,Google,Vercel secondary;
    class Supabase database;
```

---

## Featured Projects

### Sheetful
Turn your Google Sheets into powerful REST APIs in seconds.
- **Instant APIs**: GET, POST, PUT, DELETE endpoints generated automatically.
- **Secure**: Authentication and role-based access control.
- **Scalable**: Built on top of Supabase and Vercel.


---

## Contact

Feel free to explore our repositories and contribute!

[![Website](https://img.shields.io/badge/Website-sheetful.co-blue?style=flat-square&logo=google-chrome)](https://sheetful.co)
