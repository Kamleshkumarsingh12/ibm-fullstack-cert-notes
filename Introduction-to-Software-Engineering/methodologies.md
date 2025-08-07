# Software Development Methodologies

A comparison of popular SDLC models, their phases, pros/cons, and use cases.

---

## 🔹 Traditional Models

### 1. **Waterfall Model** (Linear Sequential)
```mermaid
graph LR
    A[Requirements] --> B[Design] --> C[Implementation] --> D[Testing] --> E[Deployment] --> F[Maintenance]
```
Pros: Simple, well-documented, fixed scope.
Cons: No flexibility, late testing, hard to change requirements.
Use Case: Stable requirements (e.g., government projects).

2. V-Model (Verification & Validation)
```mermaid
graph TD
    A[Requirements] --> B[System Design] --> C[Architecture Design] --> D[Module Design]
    D --> E[Coding]
    E --> F[Unit Testing] --> G[Integration Testing] --> H[System Testing] --> I[UAT]
    I --> J[Deployment]
```
