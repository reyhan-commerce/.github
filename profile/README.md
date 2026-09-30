<div align="center">

# 🌿 Reyhan Commerce

### Next-Generation Enterprise Headless E-Commerce Framework
**Powered by Laravel 13 (Octane/FrankenPHP) & Nuxt 4 (Vue 3 SSR & Tailwind v4)**

[![License: MIT](https://img.shields.io/badge/License-MIT-emerald.svg)](LICENSE)
[![Laravel Version](https://img.shields.io/badge/Laravel-13.x-red.svg)](https://laravel.com)
[![Nuxt Version](https://img.shields.io/badge/Nuxt-4.x-green.svg)](https://nuxt.com)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-17%2B-blue.svg)](https://www.postgresql.org)
[![Redis](https://img.shields.io/badge/Redis-7%2B-orange.svg)](https://redis.io)

</div>

---

## ⚡ Quick Start

Scaffold a full-stack, production-ready headless store with zero global dependencies:

```bash
npx create-reyhan@latest my-store
# or with pnpm
pnpm create reyhan my-store
```

---

## 🏛️ Core Architecture Principles

1. **Decoupled (Headless) by Design:**
   - **Backend Core:** High-performance RESTful commerce engine with **Laravel 13**, **PostgreSQL 17+**, **Filament 5**, **Laravel Octane**, and **Redis**.
   - **Storefront Layer:** Server-Side Rendered (SSR) modern web app built on **Nuxt 4**, **Nuxt UI**, and **Tailwind CSS v4**.
2. **BYOD (Bring Your Own Database):**
   - Reyhan does not force local database installation. Connect seamlessly to existing PostgreSQL 17+ and Redis 7+ servers purely via `.env`.
3. **Core Isolation & Zero-Conflict Customization:**
   - Override UI components, layouts, and pages natively via Nuxt 4 Layers without touching core files.
   - Extend or swap Eloquent models via `config/reyhan.php` and drop-in custom modules into `backend/extensions/`.
4. **Zero-Downtime Safe Updates:**
   - Automated pre-update database snapshot, schema migration, cache optimization, and Octane worker reload via `./reyhan update`.

---

## 📂 Key Repositories

| Repository | Description | Status |
| :--- | :--- | :--- |
| [**reyhan-commerce/reyhan**](https://github.com/reyhan-commerce/reyhan) | The flagship monorepo: Core engine, Nuxt 4 layer, CLI orchestrator | 🚀 Active |
| [**reyhan-commerce/create-reyhan**](https://github.com/reyhan-commerce/create-reyhan) | Interactive TUI scaffolder & CLI installer (NPX) | 📦 Published |

---

<div align="center">
  <sub>Built with ❤️ for modern merchants and developers by the Reyhan Commerce Team.</sub>
</div>
