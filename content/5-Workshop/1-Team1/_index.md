---
title: "Team 1 - KFC Ordering Agent"
date: 2026-07-25
weight: 1
---

# Team 1 (First Prize AWS Track)
## Project: AI Conversational Ordering Agent for KFC

### ⭐ Key highlight

* Selected a highly practical problem: **ordering food directly within a chat application** instead of forcing users to install a dedicated app.
* Did not just jump into the solution, but started with a **case study of McDonald's failed AI Drive-through**, helping the audience understand the pain point clearly beforehand.
* The architecture was designed as **multi-channel**, easily extensible to other brands besides KFC.
* Provided calculations of **AWS costs**, latency, and scalability, not just a simple mockup demo.

---

### 💡 Idea

Building an AI Agent that enables customers to:
* Order KFC directly on Zalo/WhatsApp.
* No app download required.
* Natural language understanding (NLU).
* Automated memory of order history.
* Order verification step before submission to avoid hallucinations.

**Workflow:**

```
Chat
↓
Intent Understanding
↓
Planning
↓
Tool Calling
↓
Menu
↓
Promotion
↓
Verify
↓
Order
```

Additionally, a dashboard is provided for staff to monitor conversation logs if the AI encounters issues.

---

### 📚 Lessons Learned

#### 1. Pitching should start with the Problem
Do not open with architecture. Start with: *"McDonald's once failed because..."* => the audience immediately grasps the pain point. This is an excellent storytelling technique.

#### 2. Architecture should be modular
They built:
* Channel Adapter
* Agent Core
* Memory
* Tool
* Dashboard

=> Changing KFC to Jollibee later on only requires changing the connector. This represents a solid software architecture mindset.

#### 3. Always include a Verify step
They emphasized that AI is not always right. Thus, there is always:
```
Verify -> Customer confirms -> Submit
```
This is a very effective way to reduce hallucinations.

#### 4. Cost is also a part of the product
They calculated infrastructure cost, latency, and Amazon Bedrock cost. This makes the project feel production-ready.

---

### 💬 Presentation Feelings

This was the most balanced presentation between Business, Technical, Demo, and AWS. What I liked most was that they constantly referred back to "customer experience" instead of just boasting about how powerful the AI was. The project has high practical viability.
