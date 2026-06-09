# Ghaith Buni

Full-stack developer based in Sweden with a B.S. in Computer Science from the University of Gävle. I build production web applications and AI-powered backend systems using Python, TypeScript, and modern frameworks.

**Backend:** Python, FastAPI, Node.js, Express, REST APIs, JWT auth, SSE streaming  
**Frontend:** React, Next.js, TypeScript, Tailwind CSS  
**Databases:** PostgreSQL, SQLModel, MongoDB, Prisma  
**AI:** Claude API, OpenAI API, Groq API, multi-provider architecture  
**DevOps:** Docker, Docker Compose, Railway, Vercel, Git

---

## Projects

### AI Chatbot with Memory
A multi-provider AI chatbot API where conversations are stored in PostgreSQL. The AI remembers full context across sessions — not just the current message.

**Stack:** FastAPI, PostgreSQL, Claude/Groq/OpenAI APIs, Docker, SSE streaming

- Three AI providers (Claude, OpenAI, Groq) with a unified service layer — switch per conversation
- Real-time response streaming using Server-Sent Events, delivering word-by-word AI responses
- Conversation memory system that loads full message history and sends it to the AI with each request
- Customizable system prompts per conversation (change the AI's personality)
- Dockerized and deployed to Railway

---

### E-Commerce API
A complete e-commerce backend with cart, orders, stock management, and role-based admin access.

**Stack:** FastAPI, PostgreSQL, SQLModel, Docker

- Database transactions for order placement: validates stock, creates order items, decreases inventory, clears cart — all atomically with rollback on failure
- Order state machine with validated transitions (pending → confirmed → shipped → delivered / cancelled)
- Purchase-verified reviews: only users who bought a product can review it
- Dynamic product filtering: search by name, category, price range with pagination
- Admin role-based access control for product and order management

---
### Service Booking Platform
A TypeScript-based booking system built with clean architecture principles, live at [swediana.se](https://www.swediana.se)

**Stack:** TypeScript, Next.js, Express, MongoDB, JWT, Zustand

- Feature-based backend structure following clean architecture
- Authentication with bcrypt, JWT access/refresh tokens, and role-based guards
- Client-side session persistence and error boundaries

---

### Cleaning & Moving Service Platform
A production booking platform for a real client, live at [vilöserdet.se](https://www.vilöserdet.se)

**Stack:** Next.js, TypeScript, Node.js, Express, MongoDB, Tailwind CSS

- Built and deployed for a real business with active customer bookings
- Geolocation-based pricing, booking calendars, promotions, and discount codes
- Admin dashboard with JWT auth, refresh tokens, and role-based access control
- Form validation with Zod, optimistic UI updates, and protected routes

---



## Get in touch

[LinkedIn](https://www.linkedin.com/in/ghaith-buni/) · ghaith.buni122@gmail.com
