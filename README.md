# qr-code-gen
# Version 1 Architecture

                     INTERNET

                ┌───────────────┐
                │               │
                ▼               ▼

        app.company.com     qr.company.com
               │                 │
               ▼                 ▼

           Vercel             Backend
           Next.js          Node/Fastify
                                 │
                         ┌───────┴────────┐
                         │                │
                         ▼                ▼

                     PostgreSQL      Analytics
                      Canada         processing
                      Central


Technology Stack Considered

| Layer            | MVP                               |
| ---------------- | --------------------------------- |
| Frontend         | Next.js + TypeScript              |
| Backend          | Fastify + TypeScript              |
| QR generation    | `qrcode` / styled QR library      |
| ORM              | Drizzle or Prisma                 |
| Database         | PostgreSQL                        |
| Database hosting | Supabase initially                |
| Backend hosting  | Railway/Render/Fly/AWS-compatible |
| Frontend hosting | Vercel                            |
| Cache            | None initially                    |
| Future cache     | Redis                             |
| Authentication   | Add after core QR flow            |
| Packaging        | Docker                            |
