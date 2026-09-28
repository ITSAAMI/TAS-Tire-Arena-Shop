<div align="center">

<img src="screenshots/02-dashboard.png" alt="TAS – Tire Arena Shop dashboard" width="100%">

# TAS – Tire Arena Shop

### Tire Shop & Workshop Management System

**Stock · Sales · Workshop Services · Purchases · Expenses · Reports · Barcodes · Thermal Printing**

![Type](https://img.shields.io/badge/type-Ready--Made%20Business%20System-e0a800)
![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL%20%2F%20MariaDB-database-4479A1?logo=mysql&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind%20CSS-UI-06B6D4?logo=tailwindcss&logoColor=white)
![Price](https://img.shields.io/badge/Price-PKR%20130%2C000-0b0b0b)

</div>

---

**TAS – Tire Arena Shop** is a complete, ready-made business management system for tire shops, rim dealers
and tire & car workshops. It replaces paper registers and spreadsheets with one fast web application that
manages stock by tire size, counter sales with printed receipts, workshop job cards, supplier purchases,
daily expenses and profit reports — all from a browser, on a desktop, laptop or phone.

> **This repository is a product showcase.** It contains screenshots and documentation of the working
> system, not its source code. The screens below show the real application running with sample demo data.

---

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Modules](#modules)
- [Technology Stack](#technology-stack)
- [Screenshots](#screenshots)
- [Business Use Cases](#business-use-cases)
- [Customization](#customization)
- [Ready-Made Solution](#ready-made-solution)
- [Pricing](#pricing)
- [Contact / Development Services](#contact--development-services)

---

## Overview

Tire businesses have one problem ordinary POS software handles badly: **the same product comes in many
sizes**, and each size has its own stock, cost and selling price. TAS is built around that. Every product
(tyre, rim, tube or accessory) holds unlimited size variants, and every size has its own barcode, stock
count, cost price, sale price and low-stock alert.

On top of that catalogue, TAS runs the whole day-to-day shop:

| Daily operation | How TAS handles it |
|---|---|
| Selling tires & parts | Fast counter sale screen with barcode scanning, discounts, 5 payment methods and instant 58mm / 80mm / A4 receipts |
| Workshop work | Job cards for fitting, balancing, alignment, puncture repair and car services, with status tracking |
| Buying stock | Supplier purchases with bill numbers; stock and cost prices update automatically |
| Running costs | Daily expense book by category (rent, salaries, utilities, fuel …) |
| Knowing the numbers | Live dashboard plus six printable, CSV-exportable reports including gross and net profit |

---

## Key Features

**Inventory & Stock**
- Products with **unlimited size variants** (e.g. 195/65/15, 205/55/16), each with its own stock, cost and sale price
- Product types (Tyre, Rim, Tube, Accessories) and brands, fully editable
- **Low-stock alerts** per size with a configurable threshold
- Automatic stock deduction on sale and addition on purchase; **overselling is blocked**
- Search by name, brand, size or barcode, with filters by type, brand, status and low stock

**Sales & Billing**
- Point-of-sale screen: scan or pick items, walk-in / existing / new customer, discount, payment method
- Payment methods: Cash, Bank Transfer, Card (POS), Easypaisa / JazzCash, Credit
- Auto-numbered invoices (`INV-000001` …)
- **Thermal receipts** (58mm & 80mm) and **A4 invoices** with business letterhead and an invoice barcode
- Editing or deleting a sale automatically corrects stock

**Workshop / Service Management**
- Service job cards with vehicle number & model, multiple services, quantities and discount
- Status workflow: **Pending → In Progress → Completed / Cancelled**
- Editable service catalogue with standard prices (tyre and car services)
- Thermal and A4 job-card printing

**Barcodes & Scanning**
- Automatic **EAN-13** (GS1 in-store range) or **Code 128** barcode for every size
- Works with any USB / Bluetooth barcode scanner — no drivers needed
- Scan from any page to open the product instantly; scan on sale/purchase screens to add items
- **Barcode label printing** on thermal rolls, custom sticker sizes or A4 sheets

**Customers, Suppliers & Purchases**
- Customer records with phone, vehicle number, address and **complete purchase & service history**
- Supplier directory and purchase entry with supplier bill / reference numbers
- Optional automatic update of cost prices from the latest purchase

**Expenses, Dashboard & Reports**
- Daily expense tracking by category with per-category and per-day totals
- **Live dashboard** (auto-refresh): today's sales, services, expenses, purchases and net; 7-day chart;
  stock snapshot; recent sales; open jobs; low-stock alerts
- Reports: **Business Summary (profit & loss)**, Sales, Purchases, Services, Expenses, Stock valuation
- Date presets (today, this week, this month, last month, this year), **print** and **CSV export**

**Administration & Security**
- Role-based access: **Admin** (full control) and **Staff** (day-to-day entry only)
- User management, account activation / deactivation, self-service password change
- Business profile (name, tagline, address, phone, email, tax number, currency) used on every document
- Hashed passwords, CSRF protection on every form, login throttling, prepared SQL statements
- Responsive layout that works on desktop, tablet and mobile

---

## Modules

| # | Module | Purpose |
|---|---|---|
| 1 | **Dashboard** | Real-time overview of the shop's day and month |
| 2 | **Stock Management** | Products, size variants, prices, stock levels and low-stock alerts |
| 3 | **Scan Barcode** | Instant product lookup by scanner or typed code |
| 4 | **Barcode Labels** | Print shelf / product labels in bulk |
| 5 | **Sales** | Counter sales, invoices, thermal & A4 receipts |
| 6 | **Services** | Workshop job cards and the service price catalogue |
| 7 | **Customers** | Customer database with full history |
| 8 | **Purchases** | Stock purchases from suppliers |
| 9 | **Suppliers** | Supplier directory |
| 10 | **Expenses** | Daily expense book by category |
| 11 | **Reports** | Profit & loss, sales, purchase, service, expense and stock reports |
| 12 | **Settings** | Business info, receipts & thermal printer, barcodes & labels, scanner, master lists |
| 13 | **Users** | Staff accounts and roles |
| 14 | **My Account** | Profile and password |

---

## Technology Stack

| Layer | Technology |
|---|---|
| Backend | PHP 8 (no heavy framework — fast on any standard hosting) |
| Database | MySQL / MariaDB with foreign keys, indexes and automatic schema upgrades |
| Frontend | Tailwind CSS, vanilla JavaScript (bundled locally — works without internet) |
| Barcodes | Built-in EAN-13 / Code 128 SVG generator |
| Printing | Dedicated print layouts for 58mm / 80mm thermal printers and A4 |
| Hardware | Any HID (keyboard-mode) USB / Bluetooth barcode scanner, any thermal receipt printer |
| Hosting | Local PC / shop LAN (XAMPP / WAMP) or any shared, VPS or cloud host |

---

## Screenshots

> All screenshots show the working application with **fictional demo data**. Names, phone numbers,
> addresses and amounts are samples only.

### 1. Login & Dashboard

| Login | Dashboard |
|---|---|
| ![Login](screenshots/01-login.png) | ![Dashboard](screenshots/02-dashboard.png) |

**Full dashboard** — KPI cards, 7-day sales / services / expenses chart, stock snapshot, recent sales, open service jobs and low-stock alerts:

![Dashboard – full view](screenshots/03-dashboard-full.png)

### 2. Stock & Inventory

**Stock management** — every product with its size variants, stock per size (low sizes highlighted in red) and price range:

![Stock management](screenshots/04-stock-products.png)

| Search (by size "205") | Low-stock filter |
|---|---|
| ![Stock search](screenshots/05-stock-search.png) | ![Low stock filter](screenshots/06-stock-low-stock-filter.png) |

| Product details | Add product |
|---|---|
| ![Product details](screenshots/07-product-details.png) | ![Add product form](screenshots/08-add-product-form.png) |

**Edit product with size variants** — each size has its own barcode, cost, sale price, stock and alert level:

![Edit product with size variants](screenshots/09-edit-product-size-variants.png)

### 3. Barcodes & Labels

| Scan barcode – instant lookup | Barcode label printing |
|---|---|
| ![Barcode lookup](screenshots/10-barcode-scan-lookup.png) | ![Barcode labels](screenshots/11-barcode-labels.png) |

**Label print preview** (80mm thermal roll):

![Label print preview](screenshots/12-barcode-labels-print-preview.png)

### 4. Sales & Billing

**Sales list** — date / payment filters, totals and discounts:

![Sales list](screenshots/13-sales-list.png)

| Sales search | New sale (POS) with scanned items |
|---|---|
| ![Sales search](screenshots/14-sales-search.png) | ![New sale POS](screenshots/15-new-sale-pos.png) |

**Sale saved** — invoice with print options (thermal / A4), edit and delete:

![Sale details](screenshots/16-sale-saved-details.png)

| A4 invoice (print view) | 80mm thermal receipt |
|---|---|
| ![A4 invoice](screenshots/17-sale-invoice-a4-print.png) | ![Thermal receipt](screenshots/18-sale-thermal-receipt.png) |

### 5. Workshop Services

**Service jobs** — job cards with vehicle, services, status and totals:

![Service jobs](screenshots/19-service-jobs.png)

| Filter by status | New service job |
|---|---|
| ![Service status filter](screenshots/20-service-jobs-status-filter.png) | ![New service job](screenshots/21-new-service-job.png) |

| Job card details | Thermal job receipt |
|---|---|
| ![Service job details](screenshots/22-service-job-details.png) | ![Service thermal receipt](screenshots/23-service-job-thermal-receipt.png) |

**Service catalogue** — tyre & car services with standard prices:

![Service catalog](screenshots/24-service-catalog.png)

### 6. Customers

![Customers](screenshots/25-customers.png)

| Customer search | Add customer |
|---|---|
| ![Customer search](screenshots/26-customers-search.png) | ![Add customer](screenshots/28-add-customer-form.png) |

**Customer profile** — contact details plus complete purchase and service history:

![Customer profile](screenshots/27-customer-profile-history.png)

### 7. Purchases & Suppliers

![Purchases](screenshots/29-purchases.png)

| New purchase (scanned items) | Purchase details |
|---|---|
| ![New purchase](screenshots/30-new-purchase.png) | ![Purchase details](screenshots/31-purchase-details.png) |

**Suppliers:**

![Suppliers](screenshots/32-suppliers.png)

### 8. Expenses

![Expenses](screenshots/33-expenses.png)

**Add expense:**

![Add expense](screenshots/34-add-expense.png)

### 9. Reports

**Business Summary** — sales revenue, cost of goods sold, gross profit, service revenue, expenses, purchases and **net profit**, with a daily breakdown:

![Business summary report](screenshots/35-report-business-summary.png)

| Sales report | Purchase report |
|---|---|
| ![Sales report](screenshots/36-report-sales.png) | ![Purchase report](screenshots/37-report-purchases.png) |

| Service report | Expense report |
|---|---|
| ![Service report](screenshots/38-report-services.png) | ![Expense report](screenshots/39-report-expenses.png) |

| Stock valuation report | Printed report (A4) |
|---|---|
| ![Stock report](screenshots/40-report-stock.png) | ![Report print view](screenshots/41-report-print-view.png) |

### 10. Settings

| Business information | Receipts & thermal printer |
|---|---|
| ![Business settings](screenshots/42-settings-business.png) | ![Receipt settings](screenshots/43-settings-receipts-thermal.png) |

| Barcodes & labels | Barcode scanner |
|---|---|
| ![Barcode settings](screenshots/44-settings-barcodes-labels.png) | ![Scanner settings](screenshots/45-settings-scanner.png) |

**Master lists** — product types, brands and expense categories:

![Lists](screenshots/46-settings-lists.png)

### 11. Users & Account

| User management (roles & status) | My account |
|---|---|
| ![User management](screenshots/47-user-management.png) | ![My account](screenshots/48-my-account.png) |

### 12. Mobile / Responsive

<p>
  <img src="screenshots/49-mobile-dashboard.png" alt="Mobile dashboard" width="300">
  &nbsp;&nbsp;
  <img src="screenshots/50-mobile-navigation.png" alt="Mobile navigation" width="300">
</p>

---

## Business Use Cases

- **Tire & rim shops** — sell by exact size, never lose track of which sizes are running low
- **Tire & car workshops** — manage fitting, balancing, alignment and repair jobs from job card to receipt
- **Tire wholesalers / distributors** — track supplier purchases, stock value and margins per size
- **Auto parts & accessories stores** — the same size-variant model works for any product with variants
- **Multi-staff shops** — owners see profit reports; staff only record day-to-day entries
- **Owners who want clarity** — one screen shows today's sales, services, expenses and net cash

---

## Customization

TAS is a ready-made sample system. **A similar solution can be developed and delivered according to your
business requirements.** You can request:

- **A similar system** for your own shop or a related business type
- **Custom branding** — your business name, logo, colours, receipts and documents
- **Custom features** — e.g. credit / ledger accounts, installments, warranty tracking, quotations
- **Database customization** — your own product structure, fields and data import from existing records
- **Business-specific modules** — multi-branch, inventory transfers, HR / payroll, loyalty, SMS / WhatsApp invoices
- **Deployment & setup** — installation on your PC, shop network, or online hosting, with printer & scanner setup
- **Additional functionality** — new reports, integrations, mobile app, online payments and more

Every business is different, so features, branding and data structure are adjusted to your workflow
before delivery.

---

## Ready-Made Solution

The complete system shown above is available as a ready-made solution that can be set up for your shop:

- ✅ All modules shown in the screenshots
- ✅ Branding with your business name, logo and contact details on screens, receipts and reports
- ✅ Installation & setup on your computer or hosting
- ✅ Thermal printer and barcode scanner configuration
- ✅ Initial product, service and expense-category setup
- ✅ Admin and staff user accounts

---

## Pricing

<div align="center">

### Complete TAS – Tire Arena Shop System — **PKR 130,000**

</div>

| Package | Price |
|---|---|
| **Ready-Made Solution** — complete TAS system with your branding, installation & setup | **PKR 130,000** |
| Additional customization, new modules or integrations | Quoted separately according to requirements |

---

## Contact / Development Services

TAS – Tire Arena Shop is designed and developed by **[LogicGigs.com](https://logicgigs.com)** — a software
house building custom business software and technology solutions.

Want this system for your shop, or a similar system built for your business?

**🌐 Website:** [https://logicgigs.com](https://logicgigs.com)

We develop custom management systems for retail shops, workshops, distributors, clinics, schools and other
businesses — from ready-made solutions like TAS to fully customized software.

---

<div align="center">

© LogicGigs.com · TAS – Tire Arena Shop. All rights reserved.<br>
<sub>Screenshots use fictional demo data. This repository is a product showcase and does not include source code.</sub>

</div>
