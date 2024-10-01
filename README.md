# Inventory Control Management

## Overview
The **Inventory Control Management** system is designed to efficiently manage and track inventory for businesses. This project provides a comprehensive database schema to handle user logins, suppliers, product items, and purchase orders. The system aims to streamline inventory management processes and enhance data organization.

## Features
- User login management with secure authentication.
- Supplier information tracking.
- Detailed product item management.
- Purchase order management, including order status and delivery tracking.
- Structured data organization using entity relationship diagrams (ERDs).

## Technologies Used
- **Database Management**: PostgreSQL / MySQL (or any DBMS you used)
- **Programming Languages**: SQL
- **Data Modeling Tools**: UML, ERD
- **Frameworks**: [If applicable, mention any frameworks or libraries used]

## Database Schema
The following tables are included in the inventory control management schema:
1. **user_login**: Stores user credentials and information.
2. **supplier**: Contains supplier details.
3. **product_items**: Manages product information, including descriptions and supplier links.
4. **purchase_orders**: Tracks purchase orders and their statuses.

### Example SQL Code
```sql
DROP SCHEMA IF EXISTS inventory_control_management CASCADE;
CREATE SCHEMA IF NOT EXISTS inventory_control_management;

CREATE TABLE IF NOT EXISTS inventory_control_management.user_login (
    user_id TEXT PRIMARY KEY,
    user_password TEXT,
    first_name TEXT,
    last_name TEXT,
    sign_up_on DATE,
    email_id TEXT
);
