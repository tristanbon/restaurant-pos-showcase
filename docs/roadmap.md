# Mini POS Roadmap

This roadmap outlines the planned development of the Mini POS System. Features are categorized by development status.

---

## ✅ Completed

### Core POS
- [x] Product browsing
- [x] Category filtering
- [x] Product search
- [x] Shopping cart
- [x] Quantity management
- [x] Product variants (sizes)
- [x] Product add-ons
- [x] Kitchen notes per item
- [x] Order summary

### Order Management
- [x] Create orders
- [x] Dine-in orders
- [x] Take-out orders
- [x] Delivery orders
- [x] Order number generation
- [x] Order list with search/filtering
- [x] Order details view
- [x] Admin order management (filter by status, payment, type, table, cashier, date)
- [x] CSV export of orders

### Table Management
- [x] Table selection
- [x] Table availability
- [x] Occupied table tracking
- [x] Cleaning status
- [x] Add tables (number, name, capacity)
- [x] Manual table status management

### Kitchen
- [x] Kitchen Order Ticket (KOT) generation and printing

### Payment
- [x] Cash payment
- [x] Automatic change calculation
- [x] GCash payment
- [x] Pay Later status
- [x] Configurable payment methods (settings)

### Discounts & Tax
- [x] Senior Citizen discount
- [x] PWD discount
- [x] Configurable discount rules (percentage/fixed, VAT-exempt, ID required)
- [x] Configurable tax rules (VAT-inclusive/exclusive)

### Receipt
- [x] Printable receipt
- [x] Transaction summary
- [x] Receipt customization (header, footer, prefix, numbering, paper size, logo)

### Reporting
- [x] Sales dashboard (today's sales, orders, average order value)
- [x] Sales trend chart
- [x] Sales by category
- [x] Top-selling products
- [x] Recent transactions
- [x] Daily / weekly / monthly / yearly reports
- [x] CSV export of reports

### Employees & Settings
- [x] User accounts with Admin / Cashier roles
- [x] Business info settings
- [x] System preferences (language, date format, low-stock threshold, order sound)
- [x] Manual database backups

---

## 🚧 In Progress

### Employee Accountability
- [ ] **Activity logs** — track admin and cashier actions (logins, edits, voids, refunds)

### Inventory
- [ ] **Stock-in for products** — record incoming stock and update available quantity
- [ ] Ingredient inventory
- [ ] Stock deduction on sale
- [ ] Low stock alerts (threshold already configurable in Preferences)

### Payment
- [ ] Card payment

### Restaurant Operations
- [ ] Order editing
- [ ] Order cancellation
- [ ] Split bills
- [ ] Merge tables

### Product Management
- [ ] Product availability toggle tied to stock

---

## 📅 Planned

### Customer
- [ ] Customer profiles
- [ ] Loyalty points
- [ ] Customer history

### Employees
- [ ] Permission management (granular, beyond Admin/Cashier roles)

### Discounts
- [ ] Coupon support
- [ ] Promotional discount scheduling

### Notifications
- [ ] Low stock notifications
- [ ] Daily sales summary

---

## 🔮 Future Enhancements

- QR Code Ordering
- Kitchen Display System (KDS)
- Online Ordering
- Delivery Module
- Mobile POS
- Multi-branch Support
- Cloud Synchronization
- Barcode Scanner Support
- BIR-compliant Official Receipt Printing
- Payment Gateway Integration
- Customer Feedback Module

---

## Version Goals

### Version 1.0 — Completed
- Stable POS with variants, add-ons, and kitchen notes
- Table Management
- Order Management
- Kitchen Order Ticket (KOT)
- Payments, Discounts & Tax
- Receipts
- Sales Dashboard & Reports
- User Management & Settings

### Version 1.5
- Inventory (stock-in, stock deduction, low stock alerts)
- Activity logs
- Order editing, cancellation, split bills
- Card payment

### Version 2.0
- Kitchen Display
- Online Ordering
- Multi-branch Support
