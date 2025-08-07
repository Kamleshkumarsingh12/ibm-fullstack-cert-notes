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
Pros: Early testing, high discipline.
Cons: Rigid, costly changes.
Use Case: Critical systems (e.g., medical software).


🔹 Iterative & Incremental Models
3. Agile (Scrum, Kanban)
```mermaid
graph LR
    A[Sprint Planning] --> B[Development] --> C[Daily Standups] --> D[Sprint Review] --> E[Retrospective] --> A
```
Pros: Flexible, customer feedback, fast delivery.
Cons: Requires active user involvement, less predictable.
Use Case: Dynamic projects (e.g., startups, SaaS).

4. Spiral Model (Risk-Driven)
```mermaid
graph LR
    A[Planning] --> B[Risk Analysis] --> C[Engineering] --> D[Evaluation] --> A
```
Pros: Handles risks, combines Waterfall + Agile.
Cons: Complex, expensive.
Use Case: High-risk projects (e.g., aerospace).


🔹 Hybrid & Modern Models
5. DevOps (CI/CD Pipeline)
```mermaid
graph LR
    A[Plan] --> B[Code] --> C[Build] --> D[Test] --> E[Deploy] --> F[Operate] --> G[Monitor] --> A
```
Pros: Faster releases, automation.
Cons: Cultural shift needed.
Use Case: Cloud-native apps (e.g., microservices).

6. RAD Model (Rapid Application Development)
```mermaid
graph LR
    A[Requirements] --> B[Prototyping] --> C[Feedback] --> D[Final Product]
```
Pros: Quick prototypes, user involvement.
Cons: High dependency on skilled teams.
Use Case: UI-heavy apps (e.g., e-commerce).


📊 Comparison Table
Model	   Flexibility	      Testing Phase	     User Feedback	   Risk Management	    Best For
Waterfall	❌Low	              Late	          Minimal	           ❌	            Stable Projects
V-Model	    ❌Low	            Parallel	      Minimal	        ⚠️ Medium	        Critical Systems
Agile	    ✅High	           Continuous	     ✅Frequent	         ✅High	           Dynamic Projects
Spiral	  ⚠️Medium	           Iterative	    ⚠️ Occasional	     ✅ High	       High-Risk Projects
DevOps	   ✅High	           Automated	    ✅ Continuous	     ✅ High	          Cloud/CI-CD
