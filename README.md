<div align="center">

<img src="images/banner.png" alt="Restaurant POS Banner" width="100%">

# Restaurant POS System

**A modern Restaurant Point of Sale (POS) System**
Built with CodeIgniter 4, Bootstrap 5, jQuery, and MySQL

![PHP](https://img.shields.io/badge/PHP-8.2-777BB4?style=for-the-badge&logo=php&logoColor=white)
![CodeIgniter](https://img.shields.io/badge/CodeIgniter-4-EF4223?style=for-the-badge&logo=codeigniter&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![License](https://img.shields.io/badge/License-Private-red?style=for-the-badge)

</div>

<br>

> **Commercial Project Notice**
> The application source code is private, as this project is intended for commercial use. This repository serves as a **portfolio showcase**, highlighting the system's interface, features, architecture, and development progress.

<br>

## Table of Contents

* [Features](https://github.com/tristanbon/restaurant-pos-showcase#features)
* [Screenshots](https://github.com/tristanbon/restaurant-pos-showcase#screenshots)
* [Demo](https://github.com/tristanbon/restaurant-pos-showcase#demo)
* [System Architecture](https://github.com/tristanbon/restaurant-pos-showcase#system-architecture)
* [Technology Stack](https://github.com/tristanbon/restaurant-pos-showcase#technology-stack)
* [Documentation](https://github.com/tristanbon/restaurant-pos-showcase#documentation)
* [Roadmap](https://github.com/tristanbon/restaurant-pos-showcase#roadmap)
* [Author](https://github.com/tristanbon/restaurant-pos-showcase#author)
* [License](https://github.com/tristanbon/restaurant-pos-showcase#license)

<br>

## Features

The system (internally codenamed **Mini POS**) is designed to streamline restaurant operations through a fast, intuitive, and role-based interface split into a **Cashier Module** for front-of-house order taking and an **Admin Module** for back-office management.

### Cashier Module

| Feature | Description |
|---|---|
| **Point of Sale (POS)** | Fast, category-filtered order entry with live search and cart |
| **Product Variants & Add-ons** | Per-item sizes (e.g. Regular / Large / Double Patty) and optional add-ons |
| **Kitchen Notes** | Free-text or quick-pick notes ("no onions", "extra spicy") sent to the kitchen |
| **Table Selection & Status** | Visual table picker showing Available, Occupied, and Cleaning status in real time |
| **Order Types** | Dine In, Take Out, and Delivery workflows |
| **Kitchen Order Ticket (KOT)** | Printable, price-free kitchen copy generated per order |
| **Discounts at Checkout** | Senior Citizen, PWD, and other configurable discounts with automatic VAT-exempt handling |
| **Multiple Payment Methods** | Cash with automatic change calculation, GCash, and Pay Later |
| **Order List** | Track open, paid, and unpaid orders with totals and status |
| **Receipt Generation** | Itemized, VAT-compliant printable receipt |

### Admin Module

| Feature | Description |
|---|---|
| **Sales Dashboard** | Today's orders, sales, average order value, available tables, sales trend, and top sellers |
| **Product Management** | Add/edit products, prices, images, variants, add-ons, and kitchen-note toggles |
| **Category Management** | Organize the menu with custom names and Font Awesome icons |
| **Table Management** | Add tables, set seating capacity, and manage status (Available / Occupied / Reserved / Cleaning) |
| **Order Management** | Search and filter every order by status, payment, type, table, cashier, and date range; export to CSV |
| **Sales Reports** | Daily / weekly / monthly / yearly totals, sales trend chart, sales by category, top-selling products, and recent transactions |
| **User Management** | Add staff accounts with Admin / Cashier roles and active/inactive status |
| **Settings – Business Info** | Business name, logo, address, contact details, TIN, and currency |
| **Settings – Payment Methods** | Configure payment options (e.g. GCash account/QR) shown at checkout |
| **Settings – Tax** | Define tax rules (e.g. 12% VAT) and whether prices are tax-inclusive |
| **Settings – Discounts** | Create discount rules with percentage/fixed value, VAT-exemption, and ID requirements |
| **Settings – Receipt** | Customize header/footer text, receipt numbering/prefix, paper size, and logo display |
| **Settings – Preferences** | System language, low-stock alert threshold, date format, backups, and order sound |
| **Settings – Backups** | Trigger and review manual/automatic database backups |

📖 See [`docs/features.md`](docs/features.md) for detailed documentation.

<br>

## Screenshots

### 🧾 Cashier Module

<details open>
<summary><strong>Login & Point of Sale</strong></summary>
<br>

| Login | POS View |
|---|---|
| ![Login](images/login-form.png) | ![POS View](images/cashier-module/pos-view.png) |

</details>

<details>
<summary><strong>Table Selection & Order Building</strong></summary>
<br>

| Select Table | Table Status While Ordering |
|---|---|
| ![Select Table](images/cashier-module/select-table.png) | ![Table Order](images/cashier-module/table-order.png) |

| Add Item (Sizes, Add-ons, Kitchen Notes) | Order Summary |
|---|---|
| ![Add Item](images/cashier-module/add-item.png) | ![Order Summary](images/cashier-module/order-summary.png) |

</details>

<details>
<summary><strong>Payment & Kitchen Order Ticket</strong></summary>
<br>

| Payment (Discounts & Payment Methods) | Kitchen Order Ticket (KOT) |
|---|---|
| ![Payment](images/cashier-module/payment.png) | ![KOT](images/cashier-module/kot.png) |

</details>

<details>
<summary><strong>Receipt</strong></summary>
<br>

| Receipt (top) | Receipt (totals & footer) |
|---|---|
| ![Receipt 1](images/cashier-module/receipt1.png) | ![Receipt 2](images/cashier-module/receipt2.png) |

</details>

<details>
<summary><strong>Order List & Order Details</strong></summary>
<br>

| Order List | Order Details |
|---|---|
| ![Order List](images/cashier-module/cashier-orderlist.png) | ![Order Details](images/cashier-module/order-details.png) |

</details>

<br>

### 🛠️ Admin Module

<details open>
<summary><strong>Dashboard</strong></summary>
<br>

![Dashboard](images/admin-module/dashboard.png)

</details>

<details>
<summary><strong>Category & Product Management</strong></summary>
<br>

| Categories | Add Category |
|---|---|
| ![Categories](images/admin-module/categories/categories.png) | ![Add Category](images/admin-module/categories/add-categories.png) |

| Products | Add Product | Edit Product |
|---|---|---|
| ![Products](images/admin-module/products/products.png) | ![Add Product](images/admin-module/products/add-products.png) | ![Edit Product](images/admin-module/products/edit-products.png) |

</details>

<details>
<summary><strong>Table Management</strong></summary>
<br>

| Tables | Add Table | Manage Table Status |
|---|---|---|
| ![Table Management](images/admin-module/table/table-management.png) | ![Add Table](images/admin-module/table/add-table.png) | ![Edit Table Status](images/admin-module/table/edit-table-status.png) |

</details>

<details>
<summary><strong>Order Management</strong></summary>
<br>

![Order Management](images/admin-module/orders/orders-management.png)

</details>

<details>
<summary><strong>Sales Reports</strong></summary>
<br>

| Reports Overview | Top Selling Products |
|---|---|
| ![Reports](images/admin-module/reports/reports.png) | ![Top Selling](images/admin-module/reports/reports-top.png) |

| Recent Transactions |
|---|
| ![Recent Transactions](images/admin-module/reports/reports-recent.png) |

</details>

<details>
<summary><strong>User Management</strong></summary>
<br>

| Users | Add User |
|---|---|
| ![Users](images/admin-module/users/users.png) | ![Add User](images/admin-module/users/add-user.png) |

</details>

<details>
<summary><strong>Settings</strong></summary>
<br>

| Business Info | Tax |
|---|---|
| ![Business Info](images/admin-module/settings/settings-info.png) | ![Tax](images/admin-module/settings/tax.png) |

| Discounts | Payment Methods |
|---|---|
| ![Discounts](images/admin-module/settings/discount.png) | ![Payment Methods](images/admin-module/settings/payment-method.png) |

| Receipt | Preferences |
|---|---|
| ![Receipt Settings](images/admin-module/settings/receipt.png) | ![Preferences](images/admin-module/settings/preferences.png) |

| Backups |
|---|
| ![Backups](images/admin-module/settings/backups.png) |

</details>

<br>

## Demo

A short demonstration of the Restaurant POS workflow.

> 🎬 **Coming soon** — a walkthrough GIF will be added at `demo/demo.gif`.

<br>

## System Architecture

The system follows CodeIgniter 4's **MVC (Model-View-Controller)** architecture, separating business logic, data handling, and presentation for maintainability and scalability. The application is split into two role-based interfaces — a **Cashier Module** for order taking and an **Admin Module** for management — sharing the same authentication and database layer.

```text
Client (Browser)
      │
      ▼
Bootstrap 5 + jQuery + AJAX  ──►  Dynamic, no-reload UI updates
      │
      ▼
CodeIgniter 4 (Controllers & Routing)
      │
      ├──►  Cashier Module (POS, Tables, Orders, Payments, KOT, Receipts)
      │
      └──►  Admin Module (Dashboard, Products, Categories, Reports, Users, Settings)
      │
      ▼
Models  ──►  MySQL Database
      │
      ▼
Views  ──►  Rendered HTML Response
```

Key architectural highlights:

- **RESTful-style controllers** handling POS, orders, products, tables, and payments
- **AJAX-driven interactions** for a fast, no-reload checkout experience
- **Modular views** shared and reused across the Cashier and Admin modules
- **Role-based access** distinguishing Admin and Cashier accounts
- **Configurable business rules** (tax, discounts, payment methods, receipt format) driven by settings tables rather than hard-coded values

📖 See [`diagrams/database-tables.md`](diagrams/database-tables.md) for the current database structure.

<br>

## Technology Stack

| Category | Technology |
|---|---|
| **Backend** | PHP 8 |
| **Framework** | CodeIgniter 4 |
| **Frontend** | Bootstrap 5 |
| **JavaScript** | jQuery, AJAX |
| **Database** | MySQL |
| **Alerts/UI** | SweetAlert2 |
| **Icons** | Font Awesome |
| **Version Control** | Git & GitHub |
| **Local Development** | Laragon |

📖 See [`docs/technologies.md`](docs/technologies.md) for more information.

<br>

## Documentation

| Document | Description |
|---|---|
| [`docs/features.md`](docs/features.md) | System features and modules |
| [`docs/api.md`](docs/api.md) | API endpoints |
| [`docs/roadmap.md`](docs/roadmap.md) | Development roadmap |
| [`docs/technologies.md`](docs/technologies.md) | Technology stack |
| [`diagrams/database-tables.md`](diagrams/database-tables.md) | Database structure |

<br>

## Roadmap

**Completed**
- [x] POS Interface (search, category filters, cart, variants, add-ons, kitchen notes)
- [x] Table Management (add tables, live status, table map)
- [x] Order Management (Dine In / Take Out / Delivery, order list, filtering, CSV export)
- [x] Kitchen Order Ticket (KOT) printing
- [x] Checkout & Payment Processing (Cash, GCash, Pay Later)
- [x] Discounts (Senior Citizen, PWD, and other configurable rules with VAT exemption)
- [x] Tax Configuration (VAT-inclusive/exclusive rules)
- [x] Receipt Generation & Customization
- [x] Product & Category Management (variants, add-ons)
- [x] User Management (Admin / Cashier roles)
- [x] Sales Dashboard & Reports (trends, top sellers, recent transactions, CSV export)
- [x] Business Settings (info, payment methods, backups, preferences)

**In Progress**
- [ ] **Activity Logs** — audit trail of admin and cashier actions
- [ ] **Stock-In for Products** — inventory receiving and stock level tracking
- [ ] Card payment support

**Planned**
- [ ] Low-stock alerts and notifications
- [ ] Order editing, cancellation, and split bills
- [ ] Merge tables
- [ ] Customer profiles and order history
- [ ] Kitchen Display System (KDS)
- [ ] QR Code Ordering
- [ ] Multi-Branch Support

📖 See [`docs/roadmap.md`](docs/roadmap.md) for the complete roadmap.

<br>

## Author

**Tristan Jay G. Bon**
Web Developer | Software Developer

[![GitHub](https://img.shields.io/badge/GitHub-tristanbon-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/tristanbon)

<br>

## License

This repository is intended for **portfolio and project showcase purposes only**.

All documentation, screenshots, and design assets are © Tristan Jay G. Bon. The commercial application source code is **not included** in this repository.

<div align="center">
<sub>Built with CodeIgniter 4, Bootstrap 5, and MySQL.</sub>
</div>
