# API Documentation

This document describes the HTTP endpoints used by the Mini POS System.

Base URL

```
http://localhost:8080/
```

---

# Product API

## Get Products

**GET**

```
/api/products
```

Returns all active products.

### Query Parameters

| Parameter | Description |
|------------|-------------|
| search | Search products |
| category | Category ID |

Example

```
GET /api/products?search=burger
```

---

# POS

## Save Order

**POST**

```
/pos/saveOrder
```

### Request

```json
{
  "cart": [],
  "order_type": "Dine In",
  "table_id": 2,
  "payment_method": "Cash",
  "amount_received": 1000,
  "reference_no": ""
}
```

### Response

```json
{
  "success": true,
  "order_id": 25,
  "receipt_url": "/receipt/25"
}
```

---

## Load Products

**GET**

```
/pos/loadProducts
```

### Query Parameters

| Parameter | Description |
|------------|-------------|
| search | Product search |
| category | Category ID |

---

# Receipt

## View Receipt

**GET**

```
/receipt/{id}
```

Displays the printable receipt.

---

# Tables

## Get Tables

**GET**

```
/tables/status
```

Returns all restaurant tables with their current status.

---

## Update Table

**POST**

```
/tables/update
```

Updates table availability.

---

# Categories

## List Categories

**GET**

```
/categories
```

Returns all categories.

---





# Error Response

```json
{
    "success": false,
    "message": "Something went wrong."
}
```

---



# Authentication

Current Version

- Session Authentication

Future Version

- JWT Authentication
- API Keys