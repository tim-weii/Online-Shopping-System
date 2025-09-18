# 🛒 Online Shopping System (Clone Prototype)

[![React Native](https://img.shields.io/badge/React%20Native-0.73-blue?logo=react)](https://reactnative.dev/) 
[![Node.js](https://img.shields.io/badge/Node.js-18-green?logo=node.js)](https://nodejs.org/) 
[![MongoDB](https://img.shields.io/badge/MongoDB-6.0-brightgreen?logo=mongodb)](https://www.mongodb.com/) 
[![Stripe](https://img.shields.io/badge/Stripe-Payments-blueviolet?logo=stripe)](https://stripe.com/) 
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 🚀 Overview

This repository is a **clone prototype** of a modern **e-commerce system**, built with **React Native, Node.js/Express, MongoDB, and Stripe**.  
It simulates the core workflow of a real-world online shopping platform:  

**Browse → Cart → Checkout → Payment → Order Tracking**

⚡ The prototype was **not launched commercially**, but served as a **hands-on exploration** of bridging **business-driven system design** with **technical implementation**.  
At the time, I was fascinated by the explosive growth of e-commerce and wanted to practice designing a scalable shopping platform from scratch.  

👉 This project forced me to think **like an entrepreneur** (system scalability, business value) while building **like an engineer** (robust APIs, payment consistency, data security).  
It fundamentally changed how I evaluate **technical feasibility vs. commercial impact** in all my future projects.  

---

## 🧱 Architecture

```text
Mobile (React Native)
 ├─ UI / Navigation (Stack, Tab)
 ├─ State Management (Zustand/Redux)
 ├─ Local Storage (AsyncStorage)
 ├─ API Client (Axios + JWT Interceptors)
 └─ Stripe SDK (Card, Apple Pay, Google Pay)
              │
              ▼
Backend (Node.js / Express)
 ├─ Auth      – JWT / bcrypt
 ├─ Products  – Query, Categories, Pagination
 ├─ Orders    – Create, Track, Status Machine
 ├─ Payments  – Stripe PaymentIntent + Webhook
 ├─ Admin     – Product & Stock Management
 └─ Validation– Zod/Joi, Rate Limit, CORS
              │
              ▼
Database (MongoDB / Mongoose)
 ├─ users     – Accounts, Addresses, Roles
 ├─ products  – Prices, Inventory, Categories
 ├─ orders    – Items, Amount, Status
 └─ payments  – PaymentIntent logs (optional)
