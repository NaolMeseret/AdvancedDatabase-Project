# E-Commerce Database System

A comprehensive database design for an E-commerce platform that addresses the challenges of managing complex and large-scale data. This project highlights advanced relational principles, optimization techniques, and scalable architecture as part of the Advanced Database Systems course.

---

## 🌟 Overview

E-commerce has revolutionized the global marketplace, transforming the way businesses and consumers interact. This project tackles the critical data management challenges in E-commerce, including:

- Seamless **user management**.
- Efficient **product categorization**.
- Robust **order tracking**.
- Scalable **shopping cart management**.

Through the implementation of relational database principles, the system ensures reliability, operational efficiency, and adaptability to meet the demands of modern digital marketplaces.

---

## ✨ Features

- **User Management**: Secure user authentication and profile handling.
- **Product Categorization**: Logical grouping of products for enhanced navigation.
- **Order Processing**: Complete order tracking, including customer and delivery details.
- **Shopping Cart**: Support for multi-product carts with size and quantity options.
- **Optimization**:
  - Vertical, horizontal, and mixed fragmentation techniques for better performance in distributed environments.

---

## 📊 Database Design

### Key Tables

| **Entity Name**      | **Description**                                                                          |
| -------------------- | ---------------------------------------------------------------------------------------- |
| **UserUpload**       | Stores user-uploaded images.                                                             |
| **CustomerProducts** | Connects products to users and customers.                                                |
| **Login**            | Manages user authentication, roles, and contact information.                             |
| **OrderTable**       | Captures order details, including customer information.                                  |
| **Category**         | Organizes products into logical categories.                                              |
| **Product**          | Stores detailed product information, including attributes like price, brand, and images. |
| **Cart**             | Represents items added to a customer’s cart for purchase.                                |

### 🔗Relationships

- **Users** upload products and place orders.
- **Categories** contain multiple products, and each product belongs to a single category.
- **Carts** link orders to products, allowing for detailed tracking of customer purchases.

---

## 📐 Entity-Relationship Diagram (ERD)

The project includes an ERD to visually represent:

- Key entities.
- Relationships among users, products, orders, categories, and carts.

![ERD Placeholder](../2025ADB/DataBaseProJect2025/E-commerce.png)

---

## 💾 SQL Implementation

### Database Schema

The database schema ensures:

- **Data integrity** through primary and foreign key constraints.
- **Efficient queries** for data retrieval and updates.
- **Logical relationships** between entities for seamless functionality.

### Example Queries

- Create and populate tables such as `UserUpload`, `Login`, `CustomerProducts`, and more.
- Retrieve product details, user data, and orders using optimized queries.

```sql
-- Example: Create a table for user uploads
CREATE TABLE UserUpload (
    UserID INT PRIMARY KEY,
    Image VARCHAR(255)
);

-- Example: Insert data into the UserUpload table
INSERT INTO UserUpload (UserID, Image) VALUES (1, 'profile1.jpg');
```

---

# 🚀 Advanced Techniques

## Vertical Fragmentation

- Divides tables by columns to optimize storage and query performance.
- Example: Splitting the UserUpload table into `{UserID, Image}`.

## Horizontal Fragmentation

- Divides tables by rows based on conditions.
- Example: UserUpload is split into:
  - Fragment 1: `Users with UserID <= 2`.
  - Fragment 2: `Users with UserID > 2`.

# Mixed Fragmentation

- Combines vertical and horizontal techniques for advanced optimization.
- Example: UserUpload split into row-based fragments while retaining only `{UserID, Image}` columns.

---

# 🔧 Getting Started

## Prerequisites

- Database Software: MySQL or any other relational database system.
- Development Tools: SQL client or command-line interface.

---

# 🤝 Contributing

- **Contributions are welcome! If you have ideas for improvements or new features, feel free to submit a pull request or open an issue.**

---

# 💡 Conclusion

- `This E-commerce database design provides a robust foundation for scalable and efficient platforms. It emphasizes structured data management and performance optimization, making it a valuable tool for modern online businesses`.

---

# 🎯 Contact

#### For questions or feedback, feel free to reach out:

- Author: **Naol Meseret**
- Email: naolmes15062015@gmail.com
- GitHub: https://github.com/NaolMeseret
