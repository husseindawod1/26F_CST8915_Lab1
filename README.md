# CST8915 Lab 1: Algonquin Pet Store on Azure VM

**Student Name**: Hussein Dawod

**Student ID**: 040971906

**Course**: CST8915 Full-stack Cloud-native Development

**Semester**: Fall 2026

---

## Demo Video

🎥 [Watch Demo Video](https://www.youtube.com/watch?v=zWwCBziFmgI)

---

## Technical Explanations

### Order Service (Node.js)

Order service is responsible for processing orders made through the product catalog. It uses Node.js and Express.js because Node.js is a lightweight JavaScript runtime that is very quick at processing information. This is essential because the order service needs to process orders in a very time-efficient manner.

It fits into the microservices architecture by being the backend for orders made on the storefront. Customers make an order on the storefront, and that request goes to the order service, which then sends the order to the order queue.

### Product Service (Rust)

Product service is responsible for displaying the products for the user to use. The programming language for the product service is Rust. It is used because it is a memory-safe language, which is beneficial because it keeps ownership of the data and the references to that data clear throughout the request and response.

It fits into the microservices architecture by being what customers interact with on the storefront, browsing through different products. It also interacts with the order service in the sense that the products are listed, and through the products, customers can set up the order they want to make.

### Store Front (Vue.js)

The storefront is responsible for displaying the application to the user, the user interface. It uses Vue.js, which is a JavaScript framework. This is because it is a very fast-loading framework that has a good state management structure, similar to React.js. This keeps the information and the current data up to date.

It fits into the microservices architecture by being what the customer sees, and through that, they can browse the products and make orders. It interacts with the order service and the product service. In the product service, there is the browsing of the products on the UI itself, and in terms of the order service, the storefront allows you to make orders with the products by browsing through the product catalog.