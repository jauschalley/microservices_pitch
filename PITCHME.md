
# Microservice Book Club 

Chapter 2: Interprocess Communication in a Microservice Architecture

---

### What is IPC?

---

### One-to-one Interactions

- each client request is processed by exactly one service
- Request/Response - a service client makes a request to a service and waits for a response. The client expects the response to arrive in a timely fashion. It might event block while waiting. This is an interaction style that generally results in services being tightly coupled.
- Request/Async response - a service client sends a request to a service, which replies asynchronously. The client does not block while waiting since the service might not send the response for a long time.
- One-way notifications - a service client sends a request to a service but no reply is expected or sent.

---

### One-to-many Interactions

- each request is processed by multiple services
- Publish/subscribe - a client publishes a notification message, which is consumed by zero or more interested services
- Publish/async responses - a client publishes a request message, and then waits for a certain amount of time for responses from interested services

---

### Sychrononous Interactions

- the client expects a timely response from the service and might even block while it waits

---

### Asychronous Interactions

- the client doesn’t block and the response, if any, isn’t necessarily sent immediately

---

### Defining a Service's API

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Semantic Versioning

- Minor.Major.Patch

---

### Message Formats

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Benefits and Drawbacks of REST

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### gRPC

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Handling Partial Failures Using a Circuit Breaker Pattern

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Service Discovery

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Types of Messaging

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Messaging Channels

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Implementation

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Documenting

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Brokerless versus Broker-based Messaging

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Transactional Messenging

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Improving Availability Using Asychronous Messaging

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

![Flux Explained](https://facebook.github.io/flux/img/flux-simple-f8-diagram-explained-1300w.png)  ### Flux Design