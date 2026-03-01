# Microservices System - API Testing Evidence

## System Status
* **Docker Setup**: All containers (Gateway, Item, Order, and Payment services) are running successfully.

![Docker Status](./testing_evidence/docker_status.png)

---

## API Gateway Testing (Port 8080)
The following evidence confirms that the API Gateway is correctly routing requests to the individual microservices.

#### 🛒 Item Service
* **GET /items**: Retrieves the current item list.
  ![Item GET](./testing_evidence/item_get.png)

* **POST /items**: Adds a new item to the inventory.
  ![Item POST](./testing_evidence/item_post.png)

### 📦 Order Service
* **GET /orders**: Retrieves the list of active orders.
  ![Order GET](./testing_evidence/order_test.png)

* **POST /orders**: Creates a new order entry through the gateway.
  ![Order POST](./testing_evidence/order_post.png)

### 💳 Payment Service
* **GET /payments**: Retrieves the history of processed payments.
  ![Payment GET](./testing_evidence/payment_test.png)

* **POST /payments**: Processes a new transaction via the gateway.
  ![Payment POST](./testing_evidence/payment_post.png)