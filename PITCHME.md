
### Decomposition

Strategies for decomposing applications

---

### What is a service?

---

### What is loose coupling?

- example

- nonexample

---

### The size of a service is mostly unimportant.

---

### Decompose by business capability

- Identify business capabilities

- From business capabilties come services

---

### Decompose by sub-domain pattern

---

### Define system operations

---

### Break down by Business Capability

- Is something that a business does to create value; defines what a business does

- Define each service based around a group of related capabilities

---

### Break down by Business Capability

- They are more stable than technical requirements which means your architecture will be less in flux (in theory)

- It’s important to repeat the process of thinking about business capabilities because you may come to varying outcomes.  You will find differences and similarities and will be able to make more informed decisions from there.

---

### DDD - Domain Driven Development Model

What is the DDD Model?

---

### Two very useful concepts can be taken from DDD and applied to microservices

---

### Subdomains

Part of a domain that is DDD term for problem space.  Identified using the same approach as identifying business capabilities; analyze the business and identify the different areas of expertise.  Then end result is likely to be subdomains that are similar to the business capabilities.

---

### Bounded Context

The scope of a domain model is called its bounded context.  Includes code artifacts that implement the model.  In a microservices architecture, each bounded context is a service or a set of services.

---

### Single responsibility principle

- Each responsibility that a class has is a potential reason for that class to change.  Added responsibilities create more reasons for the class to change, creating instability.

- We want to apply SRP to our microservices to avoid constant changes and instability.

---

### Common closure principle

- Classes in a package should be closed together against the same kinds of changes.  A change that affects a package affects all of the classes in that package.

- The idea is that if two classes in a package change because of the same underlying reasons they belong in the same package, or microservice.

- This will minimize the amount of services that need to change when a business rule is changed.

---

### Obstacles

- Network latency

- Synchronous inter-process communication reduces availability

- Maintaining data consistency across services

- God classes prevent decomposition

---

### Examples

- Public Transportation App

---

### Examples

- Fake changes to test git connectivity

---