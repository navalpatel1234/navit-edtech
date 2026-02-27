# navit-edtech
A full-stack EdTech &amp; Mentorship SaaS built with Next.js and Prisma. Features a high-converting 2-step booking flow, secure payment verification, Role-Based Access Control (RBAC) Admin Dashboard, and automated email notifications.

# NAVIT - Comprehensive EdTech & Mentorship Platform 🚀

NAVIT is a production-grade, full-stack educational platform designed to streamline student preparation for competitive exams. Built entirely on the modern Next.js ecosystem, it handles everything from content delivery (Blogs & Test Series) to complex business logic like lead capture and mentorship booking.

### 🎯 Business & Technical Highlights:
* **Exly-Style Mentorship Flow:** Engineered a robust 2-step booking system that captures lead data *before* payment initiation, drastically reducing customer drop-off rates and allowing for follow-ups.
* **Role-Based Admin Dashboard:** Secure, PIN-protected command center for administrators to manage inventory (time slots), publish markdown-style blogs, and track user conversion metrics.
* **Database & ORM:** Designed relational database schemas using Prisma ORM to efficiently link Students, Bookings, and Mentorship Slots.
* **Seamless UI/UX:** Implemented a highly responsive, glassmorphism-inspired aesthetic using Tailwind CSS and Lucide Icons, ensuring a premium feel across all devices.

### 💻 Tech Stack
* **Frontend:** Next.js (App Router), React, Tailwind CSS
* **Backend:** Next.js Serverless API Routes (Node.js)
* **Database:** Prisma ORM, SQLite / PostgreSQL
* **Integrations:** Nodemailer (Automated Transactional Emails)

### ⚙️ Key System Architecture
1. **Lead Capture API:** `POST /api/leads` - Validates and reserves slot inventory using database transactions to prevent double-booking.
2. **Payment Verification:** `POST /api/confirm-booking` - Securely verifies UPI transaction IDs, generates unique Google Meet links, and dispatches automated email/SMS confirmations.
3. **Dynamic Caching:** Utilized `force-dynamic` caching strategies to ensure real-time data synchronization between the Admin Dashboard and the Student-facing client.
