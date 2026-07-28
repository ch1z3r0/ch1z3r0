<div align="center">

# `ch1z3r0`

*Learning full-stack development by building real systems, not tutorials.*

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![TailwindCSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)

</div>

---

### 🧱 What I've built

| Layer | Stack |
|---|---|
| Frontend | React + Vite, client-side routing & state management |
| Backend | Node.js / Express (ES modules), MongoDB + Mongoose |
| Admin tooling | React + TypeScript + Tailwind, separate dashboard app |
| Auth | Firebase Admin SDK, server-side token verification |
| Storage | S3-compatible object storage (Cloudflare R2) |
| Deployment | AWS, HTTPS, public domain |

### 💳 Payment integrations

Real gateway integrations, not mocked checkouts:

- **Gateway #1** — done: signed/hashed request building, popup redirect handling, transaction status polling
- **Gateway #2** — in progress: PaymentIntents + Elements-style flow
- **Gateway #3** — partial: still needs the reliability layer the first one has

---

### 🔍 Hard-earned lessons

> The stuff that doesn't show up in tutorials.

- **Env vars loading before `dotenv` does** — top-level `process.env` reads can execute before config loads. Fix: read env vars inside function bodies, not module scope.
- **Stale closures in polling loops** — `useEffect` captures state at creation time. Live values need `useRef`, not `useState`.
- **"Success" isn't one event** — a third party confirming success and my app recording it are two separate failure domains. Worth tracking as its own case.
- **Order of operations matters** — multi-step mutations (like inventory changes) need validate-before-commit, with a defined rollback path if a later step fails.
- **Client timeouts don't cancel anything server-side** — a slow request can still complete after the UI has stopped waiting on it.
- **Sandboxes lie a little** — some real-world states (specific failure responses, edge cases) only ever show up in production.

---

### 🛠 How I work

I write the code myself first, then bring it back for review — not looking for solutions handed to me. I want the *why* before the *what*.

<div align="center">

`React` · `Vite` · `TypeScript` · `Node.js` · `Express` · `MongoDB` · `Firebase` · `Tailwind CSS` · `AWS`

</div>
