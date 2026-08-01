# Features

This document describes the core features of the Mini POS (Point of Sale) System, split into the **Cashier Module** (front-of-house order taking) and the **Admin Module** (back-office management).

---

## Cashier Module

### Point of Sale (POS)

The POS interface enables cashiers to efficiently process customer orders through a modern and responsive interface. Products can be searched instantly, filtered by category, and added to the cart with adjustable quantities. The system automatically calculates subtotals and the order total before checkout.

**Key Capabilities**
- Product search with real-time filtering
- Category-based product browsing
- Cart management with quantity adjustment
- Product variants (e.g. Regular / Large / Double Patty), each with its own price
- Optional paid or free add-ons per item
- Optional kitchen notes per item (free text or quick-pick tags)
- Automatic total calculation
- Responsive interface

### Order Types & Table Management

Orders can be placed as **Dine In**, **Take Out**, or **Delivery**. Dine In orders are linked to a table selected from a live table map showing **Available**, **Occupied**, and **Cleaning** status, along with seating capacity.

**Key Capabilities**
- Visual table selection with live status
- Occupied-table preview (current order number, customer, total)
- Automatic status handling as orders open and close

### Kitchen Order Ticket (KOT)

A price-free kitchen copy can be generated and printed per order, showing item names, sizes, add-ons, and kitchen notes so the kitchen always has an up-to-date ticket.

### Order List

Cashiers can view all open orders for their shift, including paid/unpaid counts and total sales, with search and filtering by order number, payment status, order type, and date.

### Payment Processing

The payment module supports multiple payment methods and streamlines the checkout process. Discounts can be applied at checkout, and cash payments calculate change automatically.

**Key Capabilities**
- Cash payment with automatic change calculation
- GCash and Pay Later options
- Discount application (e.g. Senior Citizen, PWD) with automatic VAT-exempt recalculation
- Payment status tracking

### Receipt Generation

After a successful payment, the system generates a printable, VAT-compliant receipt containing the order summary, purchased items, discounts, tax breakdown, payment information, and transaction details.

**Key Capabilities**
- Printable receipt
- Order summary with itemized add-ons and variants
- VAT-exempt / VAT-inclusive breakdown
- Payment details and change amount
- Transaction record

---

## Admin Module

### Dashboard

A real-time overview of restaurant performance, including today's orders, sales, average order value, available tables, a sales trend chart, and the top-selling products for the period.

### Product Management

Add, edit, and organize menu items, including images, pricing, variants, add-ons, and whether kitchen notes are allowed for that item.

### Category Management

Group products into categories with a custom name and Font Awesome icon for faster navigation in the POS.

### Table Management

Add tables with a table number, name, and seating capacity, and manage their status (Available, Occupied, Reserved, Cleaning). Occupied status is automatically managed by the POS as orders are opened and closed.

### Order Management

View, search, and filter every order across the restaurant by order status, payment status, order type, table, cashier, and date range, with CSV export for reporting.

### Sales Reports

Monitor revenue, orders, products sold, and business performance over Today / This Week / This Month / This Year ranges, including:
- Sales trend chart
- Sales by category
- Top-selling products (quantity sold and revenue)
- Recent transactions
- CSV export

### User Management

Add and manage staff accounts with Admin or Cashier roles, active/inactive status, and login tracking.

### Settings

System-wide configuration, organized into tabs:

| Tab | Description |
|---|---|
| **Business Info** | Business name, logo, address, contact number, email, TIN, and currency — used across receipts and the admin panel |
| **Payment Methods** | Configure payment options available at checkout (e.g. GCash account details and QR code) |
| **Tax** | Define tax rules (e.g. 12% VAT) and whether listed prices already include tax |
| **Discounts** | Create discount rules (percentage or fixed) with VAT-exemption and ID-requirement flags |
| **Receipt** | Customize receipt header/footer text, receipt number prefix and sequence, printer paper size, and logo display |
| **Preferences** | System language, low-stock alert threshold, date format, automatic backups, and order notification sound |
| **Backups** | Trigger a manual backup and review backup history |

---
