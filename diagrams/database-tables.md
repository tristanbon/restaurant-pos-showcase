# Database Structure

The Mini POS database is organized around four areas: **catalog** (what's sold), **operations** (orders, tables, payments), **configuration** (business/tax/discount/receipt settings), and **accounts** (users). This reflects the current schema; no source code or raw data is included in this showcase.

---

## Catalog

| Table | Purpose |
|---|---|
| `categories` | Menu categories (name + Font Awesome icon) used to group products |
| `products` | Menu items — name, base price, category, image, and flags for variants/add-ons/kitchen notes |
| `product_variants` | Per-product size/option pricing (e.g. Regular, Large, Double Patty) |
| `product_addons` | Per-product optional add-ons and their price |

## Operations

| Table | Purpose |
|---|---|
| `restaurant_tables` | Tables — number, name, seating capacity, and live status (Available / Occupied / Reserved / Cleaning) |
| `orders` | Order header — type (Dine In / Take Out / Delivery), table, cashier, totals, discount, tax, payment status, order status |
| `order_items` | Line items per order — product, variant, add-ons, quantity, price, and kitchen notes |
| `payments` | Payment records per order — method, amount received, change, and reference number |

## Configuration

| Table | Purpose |
|---|---|
| `business_settings` | Business name, logo, address, contact info, TIN, and currency |
| `payment_methods` | Configurable payment options available at checkout (e.g. GCash account + QR) |
| `tax_settings` | Tax rules (name, rate, whether prices already include tax) |
| `discount_rules` | Discount definitions (name, type, value, VAT-exemption, ID requirement, active status) |
| `receipt_settings` | Receipt header/footer text, numbering/prefix, paper size, and logo display |
| `system_preferences` | Key/value system-wide preferences (language, low-stock threshold, date format, etc.) |
| `backup_logs` | History of manual/automatic database backups |

## Accounts

| Table | Purpose |
|---|---|
| `users` | Staff accounts — name, email, role (Admin/Cashier), status, and login/lockout tracking |
| `user_tokens` | Tokens for email verification, password reset, and two-factor flows |

---

## Planned Additions

These tables support the **In Progress** roadmap items and are not yet part of the schema:

- `activity_logs` — audit trail of admin and cashier actions
- Inventory tables (e.g. `ingredients`, `stock_movements`) — to support stock-in and stock deduction for products

📖 See [`docs/roadmap.md`](../docs/roadmap.md) for the full roadmap.
