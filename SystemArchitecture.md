##  4. `docs/SystemArchitecture.md`

# System Architecture – Mitomba eSales

## Components
- Trader Interface– uploads, dashboard
- Buyer Interface – browse, buy, track
- Backend– handles auth, products, orders, payments
- Payment Gateway – M-Pesa or MoMo integration

##  Data Flow
1. Trader uploads product
2. Buyer browses → adds to cart → orders
3. Payment processed
4. Notification sent
5. Order recorded in DB

##  Database Schema (Simplified)
Users
- id, name, email, type (buyer/trader)

Products
- id, trader_id, image_url, name, price, description

Orders
- id, buyer_id, product_id, status, payment_status

##  API Endpoints
- `POST /register`
- `POST /login`
- `GET /products`
- `POST /orders`
- `POST /pay`
