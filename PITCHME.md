
# Microservice Book Club 

Chapter 2: Interprocess Communication in a Microservice Architecture

---

### What is IPC?

---

### One-to-one Interactions

- each client request is processed by exactly one service

---

### One-to-one Interactions

- Request/Response - a service client makes a request to a service and waits for a response. The client expects the response to arrive in a timely fashion. It might event block while waiting. This is an interaction style that generally results in services being tightly coupled.

---

### One-to-one Interactions

- Request/Async response - a service client sends a request to a service, which replies asynchronously. The client does not block while waiting since the service might not send the response for a long time.

---

### One-to-one Interactions

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

---

### Semantic Versioning

- Minor.Major.Patch
- Minor, backwards-compatible changes
- Major, breaking changes

---

### Message Formats

---

### Benefits and Drawbacks of REST

---

### gRPC

-gRPC is a framework for writing cross-language RPC clients and servers

---

### Handling Partial Failures Using a Circuit Breaker Pattern

-A circuit breaker pattern is an RPI proxy that immediately rejects invocations for a timeout period after the number of consecutive failures exceeds a specified threshold.

---

### Service Discovery

---

### Types of Messaging

---

### Messaging Channels

---

### Implementation

---

### Documenting

---

### Brokerless versus Broker-based Messaging

---

### Transactional Messenging

---

### Improving Availability Using Asychronous Messaging

---

### Summary

- The microservice architecture is a distributed architecture and so inter-process communication plays a key role

---

### Summary

- It’s essential to carefully manage the evolution of a service’s API. Backwards compatible changes are the easiest to make since they don’t impact clients. If you make a breaking change to a service’s API it will typically need to support both the old and new versions until its clients have been upgraded.

---

### Summary

- There are numerous IPC technologies, each with different trade-offs. One key design decision is to choose either a synchronous Remote procedure invocation pattern or the asynchronous Messaging pattern.

---

### Summary

- In order to prevent failures from cascading through a system, a service client that uses a synchronous protocol must be designed to handle partial failures.

---

### Summary

- An architecture that uses synchronous protocols must include a service discovery mechanism in order for clients to determine the network location of a service instance.

---

### Summary

- A good way to design a a messaging-based architecture is using the messages and channels model, which abstracts the details of the underlying messaging system.
---

### Summary

- One key challenge when using messaging is atomically updating the database and publishing a message.
---