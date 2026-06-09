<div align="center">

# 🛒 MultiCart

### Multi-Vendor E-Commerce Platform

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit-brightgreen?style=for-the-badge&logo=vercel)](https://multicart-bay.vercel.app)
[![GitHub](https://img.shields.io/badge/Source%20Code-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/iamankit04/multicart)
[![Next.js](https://img.shields.io/badge/Next.js-black?style=for-the-badge&logo=next.js)](https://nextjs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org)

A full-stack multi-vendor e-commerce platform with vendor verification, Stripe payments, OTP-based delivery, return/refund workflows, and AI-powered chat support.

</div>

---

## 📸 Overview

MultiCart is a production-grade e-commerce platform that brings together **Users**, **Vendors**, and **Admins** under one roof. Vendors can list and manage their products after admin verification, users can shop and pay securely via Stripe, and every order is protected by OTP-based delivery confirmation with a full return and refund system.

---

## ✨ Features

### 👤 User
- Browse products from multiple vendors in one place
- Secure Google OAuth & credential-based login (JWT sessions)
- Stripe-powered checkout with OTP-verified delivery confirmation
- Request returns and refunds with order tracking

### 🏪 Vendor
- Submit business details (Shop Name, GST, Address) for admin approval
- Manage product listings, inventory, and orders
- AI-powered chat support with users and admin
- Role-restricted dashboard access post-verification

### 🛡️ Admin
- Review and approve/reject vendor verification requests
- Platform-wide order, product, and user management
- AI-powered chat with vendors
- Full access control and oversight dashboard

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | Next.js, TypeScript, Tailwind CSS |
| **Backend** | Next.js API Routes, Node.js |
| **Database** | MongoDB, Mongoose |
| **Auth** | NextAuth.js (Google OAuth + Credentials + JWT) |
| **Payments** | Stripe (OTP delivery verification, returns & refunds) |
| **State Management** | Redux Toolkit (custom async hooks) |
| **AI Chat** | AI-powered support for admin-vendor & vendor-user |

---

## 🏗️ Architecture Highlights

- **Vendor Verification Flow** — Vendors submit GST and business details; admin reviews and approves before any selling access is granted
- **OTP Delivery Confirmation** — Orders are only marked delivered after the buyer enters a one-time password, preventing false deliveries
- **Return & Refund Workflow** — Structured multi-step return and refund process with Stripe integration
- **JWT Session Management** — Secure, stateless sessions via NextAuth.js with role-aware token payloads
- **Role-Based AI Chat** — AI support channels scoped per role: admin↔vendor and vendor↔user, with strict access restrictions
- **Global State** — Redux Toolkit slices for current user and vendor data with custom async hooks

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- MongoDB instance (local or Atlas)
- Stripe and NextAuth credentials

### Installation

```bash
# Clone the repository
git clone https://github.com/iamankit04/multicart.git
cd multicart

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Fill in your credentials in .env.local

# Run the development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the app.

### Environment Variables

```env
NEXTAUTH_SECRET=
NEXTAUTH_URL=

GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=

MONGODB_URI=

STRIPE_PUBLIC_KEY=
STRIPE_SECRET_KEY=
STRIPE_WEBHOOK_SECRET=
```

---

## 📁 Project Structure

```
multicart/
├── app/                  # Next.js App Router pages & API routes
│   ├── (user)/           # User-facing storefront & orders
│   ├── (vendor)/         # Vendor dashboard & product management
│   ├── (admin)/          # Admin dashboard & verification panel
│   └── api/              # API route handlers
├── components/           # Reusable UI components
├── lib/                  # DB connection, utilities, helpers
├── store/                # Redux Toolkit slices & store config
├── middleware.ts          # Role-based route protection
└── public/               # Static assets
```

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📬 Contact

**Ankit Kumar Gupta**
- 📧 [ankitkumargup143@gmail.com](mailto:ankitkumargup143@gmail.com)
- 💼 [linkedin.com/in/iamankit04](https://linkedin.com/in/iamankit04)
- 🐙 [github.com/iamankit04](https://github.com/iamankit04)

---

<div align="center">

*Built with ❤️ by Ankit Kumar Gupta*

</div>
