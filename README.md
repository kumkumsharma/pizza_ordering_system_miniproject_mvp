# 🍕 SliceMatic (Stage 2 MVP)

## Overview

This project is a command-line Pizza Ordering System developed as part of the FDE AI Engineering Program.

The application allows customers to place pizza orders by selecting a base, pizza type, topping, quantity, and payment mode. The system validates all user inputs, calculates the final bill, and stores completed orders in a structured log file.

---

## Features

- Runtime loading of menu files
- Customer name validation
- Indian mobile number validation
- Menu selection validation
- Quantity validation
- Payment mode validation
- Automatic bill calculation
- Discount calculation
- GST calculation
- Order confirmation
- Order logging in JSON format

---

## Folder Structure

```
project/

│
├── menu/
│   ├── Types_of_Base.txt
│   ├── Types_of_Pizza.txt
│   └── Types_of_Toppings.txt
│
├── logs/
│   └── orders_log.txt
│
├── pizza_ordering_system_miniproject_mvp.ipynb
│
└── README.md
```

---

## Technologies Used

- Python
- Google Colab
- JSON
- File Handling

---

## Business Rules

- Customer name accepts only alphabets and spaces.
- Mobile number must be a valid 10-digit Indian number starting with 6, 7, 8 or 9.
- Menu selections must be within the displayed range.
- Quantity must be between 1 and 10.
- Payment modes:
  - Cash
  - UPI
  - Card
- Discount:
  - 10% discount for orders with quantity ≥ 5.
- GST:
  - 18% applied after discount.

---

## Order Logging

Every completed order is appended to `orders_log.txt` as a JSON object.

Each order contains:

- Timestamp
- Customer Name
- Phone Number
- Base
- Pizza
- Topping
- Unit Prices
- Quantity
- Subtotal
- Discount
- GST
- Final Total
- Payment Mode

---

## Edge Cases Handled

- Empty customer name
- Invalid customer name
- Invalid phone number
- Phone number with incorrect length
- Invalid menu selection
- Out-of-range menu selection
- Invalid quantity
- Invalid payment mode
- Missing menu files
- Malformed menu records

---

## Future Improvements (Stage 3)

- React + Vite frontend
- Supabase PostgreSQL database
- Admin Login
- Live Order Dashboard
- AI-powered Business Insights using OpenRouter
- Deployment on Vercel

---

## Author
Kumkum Sharma