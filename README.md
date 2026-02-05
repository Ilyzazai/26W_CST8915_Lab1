# CST8915 Lab 1: Algonquin Pet Store on Azure VM

Student Name: Ilyas Zazai  
Student ID:  041173490
Course: CST8915 – Full-stack Cloud-native Development  
Semester: Winter 2026  

---

## Demo Video

YouTube Link: https://youtu.be/RpCx6Aks39A

---

## Technical Explanations

### Product Service (Rust)
The Product Service is for managing the product . It is implemented in Rust and exposes REST API and that allow other services to get product information. This service runs independently on port 3030 and is accessed by the Store Front.

---

### Order Service (Node.js)

The Order Service handles customer orders. It is built using Node.js and receives orders from the Store Front. When order is placed, the service sends a message to RabbitMQ, allowing orders to be processed.
---

### Store Front (Vue.js)

The Store Front is the client-facing web application built with Vue.js. It allows users to browse products, add items to the cart, and place orders. The Store Front communicate with the Product Service to show products and with the Order Service to submit orders.

---

## Notes
This lab shows a microservices-based/Rest API application deployed on an Azure Virtual Machine, including inter-service communication and message queuing using RabbitMQ.
