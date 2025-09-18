# 🛒 Online Shopping System (Clone Prototype)

[![React Native](https://img.shields.io/badge/React%20Native-0.73-blue?logo=react)](https://reactnative.dev/) 
[![Node.js](https://img.shields.io/badge/Node.js-18-green?logo=node.js)](https://nodejs.org/) 
[![MongoDB](https://img.shields.io/badge/MongoDB-6.0-brightgreen?logo=mongodb)](https://www.mongodb.com/) 
[![Stripe](https://img.shields.io/badge/Stripe-Payments-blueviolet?logo=stripe)](https://stripe.com/) 
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 🚀 Overview

This repository is a modern **e-commerce system clone prototype**, built with **React Native, Node.js/Express, MongoDB, and Stripe**.  
It simulates the core workflow of a real-world shopping platform:  

**Browse → Cart → Checkout → Payment → Order Tracking**

This project was **not launched commercially**, but served as a **hands-on exercise** to bridge **business-driven system design** and **technical implementation**.  
At the time, I was fascinated by the rapid growth of the e-commerce industry and wanted to practice designing a scalable platform from scratch.  

👉 It pushed me to think like an **entrepreneur** (system scalability, business value) while building like an **engineer** (robust APIs, payment consistency, data security).  
It fundamentally changed how I evaluate **technical feasibility vs. commercial impact** in future projects.  

---

## 🧱 System Architecture

```text
Mobile (React Native)
 ├─ UI / Navigation (Stack, Tab)
 ├─ State Management (Zustand)
 ├─ Local Storage (AsyncStorage)
 ├─ API Client (Axios)
 └─ Stripe SDK (Card, Apple Pay, Google Pay)
              │
              ▼
Backend (Node.js / Express)
 ├─ Auth            – JWT / bcrypt
 ├─ Products        – Query, Categories, Pagination
 ├─ Orders          – Create, Track, Status Machine
 ├─ Payments        – Stripe PaymentIntent + Webhook
 ├─ Admin           – Product & Inventory Management
 ├─ Validation      – Zod/Joi, Authentication, Authorization, Business Rules,
 │                    CORS, Rate Limiting, Webhook Signature Verification
 └─ Observability   – Logs / Metrics / Alerts
              │
              ▼
Database (MongoDB / Mongoose)
 ├─ stores    – Store accounts, owners, contact info
 ├─ users     – Accounts, roles, store affiliation, addresses, contact info
 ├─ products  – Prices, stock, categories, per-store isolation
 ├─ orders    – Items, amount, status, storeId reference
 └─ payments  – PaymentIntent logs (optional)
```
