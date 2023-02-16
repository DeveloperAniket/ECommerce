# ECommerce

## Overview
The purpose of this architecture definition is to provide a solution design and technical guidelines for ECommerce webiste name MCart. The architecture definition defines recommended design as per the requirements and constraints of SRS Document.

## Key Capabilites
- Login
- Registration
- Admin Page
- Search Products
- Product Catalogs
- Sale
- Stock
- Price
- Filter Prodcuts
- Cart Managment
- Payment System
- Order Managment

## Assumptions : 
- Application will target signle region customer only.
- Web hosting. this website that will be used to integrate an e-commerce functionality.
- Website security is another important technical aspect in e-commerce systems. A lot of sensitive information, such as credit card numbers, phone numbers, and home addresses, will be used in the e-commerce transactions. It is vital that this information remains safe from cyber criminals. The website must have a Secure Socket Layer encryption to allow secure connections.
- The solution must have a backup, routine and automatic backups must be setup. This will allow recovery from a catastrophic data loss.
- Payment gateway that will accept payments. This is a merchant service provider that accepts online credit card payments. After a customer enters their credit card information, the payment gateway authorizes the transaction and processes the payment. The payment gateway encrypts sensitive information to ensure that the information passes securely between the customer and merchant.
- System should be avaiable 24 X 7. System need to be fault tollarante. 
- Must be integrate with Shipping software that will automate the management of outgoing shipment of customer orders, create and print shipping labels, and import tracking information for orders, and generate automated customer emails.

## NFR
- Availability
- Consistency
- Latency


## System Context 
<img width="639" alt="image" src="https://user-images.githubusercontent.com/9957969/214040693-ed00ae78-904c-4adc-b8fa-4885ab82ddb6.png">

## Functional Diagram
![Untitled Diagram1](https://user-images.githubusercontent.com/9957969/219303988-c0b487fa-1e0a-4581-ab71-eb0d6edd44bc.jpg)

## User Service
- Functional  Login using facebook ,Twitter or manual registed user
- Login should have low latency , 
- Availability should be 99.9%
- Highly secure
- Strong consistency

## Product Service
- Add or Search Product
- Highly Available
- Should be follow Eventual consistency
- Low Latency

## Order Service
- Manage Order
- Highly Available
- Should be follow Strong consistency
- Low Latency

# Payment Service
- External Service 

# Logistic Service
- External Service

# Cart Service
- Manage User Cart
- Highly Available
- Should be follow Strong consistency
- Low Latency
