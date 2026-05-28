

**why production issues still happen even after lower-environment testing.**
Yes, we validate deployments in lower environments, but production still exposes edge cases because lower environments usually cannot exactly match production scale, workload, traffic patterns, infrastructure pressure, third-party dependencies, and real user behavior.
Our responsibility was to identify the issue quickly using logs, events, metrics, and monitoring, then implement preventive measures.”

**How services communicate?**
You can say: REST APIs, Internal Kubernetes services, Sometimes Kafka/RabbitMQ for async communication.

**How did pods communicate securely?**
TLS, Network policies, Internal service communication

**How did you handle sensitive customer data?** 
Need: secrets, encryption, restricted access, RBAC
