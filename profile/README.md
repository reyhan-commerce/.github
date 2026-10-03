<div align="center">

<img src="images/banner.png" alt="Reyhan Commerce Framework" width="850" style="max-width: 100%; border-radius: 14px; margin-bottom: 24px;" />

# Reyhan Commerce

### Sovereign Enterprise Headless E-Commerce Backend Framework
**Engineered for Laravel 13 with 100% Strict Typing, Action-Driven Architecture, High Concurrency & Double-Entry Financial Precision**

[![License: MIT](https://img.shields.io/badge/License-MIT-emerald.svg)](https://opensource.org/licenses/MIT)
[![Packagist: core](https://img.shields.io/packagist/v/reyhan-commerce/core.svg?label=core&style=flat-square)](https://packagist.org/packages/reyhan-commerce/core)
[![Packagist: installer](https://img.shields.io/packagist/v/reyhan-commerce/installer.svg?label=installer&style=flat-square)](https://packagist.org/packages/reyhan-commerce/installer)
[![PHP Version](https://img.shields.io/badge/PHP-8.4%20%7C%208.5-blue.svg)](https://php.net)
[![Laravel Version](https://img.shields.io/badge/Laravel-13.x-red.svg)](https://laravel.com)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-17%2B-336791.svg)](https://www.postgresql.org)
[![Redis](https://img.shields.io/badge/Redis-7%2B-dc382d.svg)](https://redis.io)
[![Documentation](https://img.shields.io/badge/Docs-Live%20Website-10b981.svg)](https://reyhan-commerce.github.io/docs/)

</div>

---

## ⚡ Quick Start

### Option A: Install via Composer Global CLI (Recommended)

Scaffold a production-ready headless store with an interactive terminal wizard powered by **Laravel Prompts**:

```bash
# 1. Install the Reyhan CLI globally
composer global require reyhan-commerce/installer

# 2. Scaffold a new store project
reyhan new my-store
```

### Option B: Direct `composer create-project`

```bash
composer create-project reyhan-commerce/reyhan my-store
cd my-store
php artisan migrate --seed
php artisan serve
```

Admin Backoffice: `http://localhost:8000/admin`  
OpenAPI / Scalar API Docs: `http://localhost:8000/docs/api`

---

## 🏛️ Ecosystem Repositories

| Repository | Packagist / Link | Primary Responsibility | Status |
| :--- | :--- | :--- | :--- |
| [**`reyhan-commerce/core`**](https://github.com/reyhan-commerce/core) | [`reyhan-commerce/core`](https://packagist.org/packages/reyhan-commerce/core) | Core framework engine library: domain facades, commercial pipelines, double-entry ledger, models & Filament admin plugin. | 🟢 Stable |
| [**`reyhan-commerce/reyhan`**](https://github.com/reyhan-commerce/reyhan) | [`reyhan-commerce/reyhan`](https://packagist.org/packages/reyhan-commerce/reyhan) | Turnkey starter application skeleton (Standard Laravel 13 layout) consuming the core framework. | 🟢 Stable |
| [**`reyhan-commerce/create-reyhan`**](https://github.com/reyhan-commerce/create-reyhan) | [`reyhan-commerce/installer`](https://packagist.org/packages/reyhan-commerce/installer) | Official Composer CLI installer & project scaffolder with interactive prompts and CI automation flags. | 🟢 Stable |
| [**`reyhan-commerce/docs`**](https://github.com/reyhan-commerce/docs) | [Live Documentation](https://reyhan-commerce.github.io/docs/) | Official documentation portal built with VitePress and deployed via GitHub Pages. | 🟢 Live |
| [**`reyhan-commerce/storefront-nuxt`**](https://github.com/reyhan-commerce/storefront-nuxt) | [Storefront Repo](https://github.com/reyhan-commerce/storefront-nuxt) | Official decoupled reactive storefront built with Nuxt 4, Vue 3, Tailwind CSS v4, and Nuxt UI. | 🚀 In Active Dev |

---

## 💎 Core Architecture Pillars

1. **Uncompromising Strict Typing & Farshid's Laravel Constitution:**
   - Mandatory `declare(strict_types=1);` across all framework code.
   - Domain mutations encapsulated in single-responsibility `final class [Verb][Noun]Action` classes with `execute()`.
   - Native Eloquent models and relationships; leaky repository patterns are strictly banned.
   - Modern attribute casting using `protected function casts(): array`.

2. **Dynamic Model Extensibility Engine:**
   - Swap or extend any core model (Product, Order, Variant, Cart, User) at runtime using `Reyhan::useModel('alias', CustomModel::class)` with seamless polymorphic relation resolution.

3. **High-Concurrency Two-Tier Inventory Guard:**
   - Eliminates overselling during high-traffic flash sales by pairing fast atomic Redis reservations with PostgreSQL pessimistic row locking (`ProductVariant::lockForUpdate()`).

4. **Double-Entry Financial Accounting Ledger:**
   - Guarantees financial balance ($\sum \text{Debit} \equiv \sum \text{Credit}$) across all wallet balances, refunds, and bank transactions.

5. **Multi-Driver Iranian Commerce Subsystems:**
   - Driver-based Shetabit bank payment gateway manager (Zarinpal, SEP, Mellat Bank, Sandbox).
   - Multi-driver transactional SMS notifications with fast pattern lines (Kavenegar, FarazSMS, Ghasedak).
   - Persian text normalization pipeline (ZWNJ, Arabic/Persian unified characters, Persian numerals).

---

## 📖 Documentation & Community

- 📚 **Official Documentation:** [https://reyhan-commerce.github.io/docs/](https://reyhan-commerce.github.io/docs/)
- 💬 **Discussions & Issues:** [GitHub Issues](https://github.com/reyhan-commerce/reyhan/issues)
- 📄 **License:** Open-sourced under the [MIT License](https://opensource.org/licenses/MIT).

<div align="center">
  <sub>Built with ❤️ for sovereign, resilient commerce by the Reyhan Commerce Team.</sub>
</div>
