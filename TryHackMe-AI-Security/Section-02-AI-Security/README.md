# TryHackMe AI Security — Section 02: AI Security

## Overview

This section focuses on the security of AI systems from an offensive and
defensive perspective.

It builds on the foundational concepts from Section 01 and introduces
security frameworks, LLM-specific threats, AI threat modelling,
AI system reconnaissance, and practical security assessment.

A major focus of this section was understanding how traditional
cybersecurity approaches can be adapted for AI systems and how AI-specific
attack surfaces require additional considerations.

---

## Rooms Covered

### 1. Securing AI Systems

This room introduced the security frameworks and approaches used to
assess modern AI systems.

A major focus was understanding:

- **OWASP Top 10 for LLM Applications**
- **MITRE ATLAS**
- AI-specific security risks
- AI system attack surfaces
- Mapping security risks to different AI system components

Learning these frameworks helped me understand how AI security can be
structured using established cybersecurity methodologies while accounting
for AI-specific threats.

---

### 2. LLM Security

This room focused on security threats affecting Large Language Models
(LLMs).

One of the areas I found particularly useful was understanding threats
from different parts of an AI ecosystem, including:

- **Database-based threats**
- **Model-based threats**
- **System-based threats**
- **User-based threats**

This helped me understand that securing an LLM is not only about
protecting the model itself.

The surrounding data, infrastructure, applications, users, and supporting
systems can all introduce security risks.

This perspective is important when assessing AI-powered applications
because vulnerabilities may exist outside the model while still affecting
the overall AI system.

---

### 3. AI Threat Modelling

This was one of the most interesting rooms in the section because it
connected traditional threat modelling concepts with AI-specific security
problems.

Key areas covered included:

- AI-specific assets
- AI attack surfaces
- Data supply chains
- Limitations of traditional STRIDE modelling for AI
- Adapting STRIDE for AI systems
- MITRE ATLAS
- OWASP LLM Top 10
- Mapping risks to AI system components
- Practical AI threat modelling

A key lesson was that traditional threat modelling frameworks can provide
a useful foundation, but AI systems introduce additional assets,
dependencies, and attack surfaces that need to be considered.

---

### 4. AI System Reconnaissance

This room introduced reconnaissance techniques specifically for AI
systems.

I particularly liked the process of identifying the technology and
infrastructure behind an AI system.

Areas of interest included:

- Port scanning
- Service discovery
- Technology fingerprinting
- Identifying exposed infrastructure
- Understanding the attack surface of AI-powered systems

This connected strongly with my existing penetration testing experience
with tools such as Nmap and helped me see how traditional reconnaissance
techniques can be applied when assessing AI systems.

AI reconnaissance is important because an AI application may expose
multiple supporting services and technologies beyond the visible
interface.

---

### 5. AI Threat Modelling Assessment

The final room acted as a practical assessment of the concepts covered
throughout the section.

The assessment consisted of two phases.

#### Phase 1 — Guided Questions

This phase tested my understanding of:

- AI system components
- AI-specific vulnerabilities
- Security risks
- Appropriate mitigations
- Threat modelling concepts

#### Phase 2 — Attack Simulation

The second phase involved practical attack scenarios against an AI system
architecture.

The task required identifying where security controls should be placed
on the architecture diagram.

The assessment required **100% completion** to pass.

**Result:**

- ✅ Completed
- ✅ 100% score
- ✅ Both flags captured

This practical assessment helped reinforce the relationship between
AI architecture, attack surfaces, threats, and security controls.

---

## Key Security Frameworks

### OWASP Top 10 for LLM Applications

The OWASP Top 10 for LLM Applications provides a structured way to
understand common security risks affecting applications that use
Large Language Models.

During this section, I focused on understanding how LLM risks can be
mapped to different components of an AI system.

This is particularly useful for application security because AI-powered
applications can inherit both traditional web vulnerabilities and
AI-specific risks.

---

### MITRE ATLAS

MITRE ATLAS provides a knowledge base for understanding adversarial
techniques against AI-enabled systems.

Learning about ATLAS helped me understand how AI attacks can be viewed
from an adversarial perspective and how techniques can be organized
within an AI-specific threat landscape.

It also provides a useful complement to traditional frameworks such as
MITRE ATT&CK when working with AI-enabled environments.

---

## AI Security Threat Categories

One of the useful concepts from the LLM Security room was looking at
threats according to the part of the ecosystem they affect.

### Database-Based Threats

Threats involving the data stores and databases supporting AI systems.

### Model-Based Threats

Threats that directly affect or target AI models and their behavior.

### System-Based Threats

Threats involving the infrastructure, applications, services, and
components surrounding the AI model.

### User-Based Threats

Threats involving users, their interactions with AI systems, and the
ways user input can influence system behavior.

This helped me move away from thinking about an AI model as an isolated
component and instead view AI security as the security of the complete
system.

---

## AI Security Reconnaissance

AI system reconnaissance was one of the areas I found particularly
interesting.

The process is similar to traditional penetration testing reconnaissance,
but the objective is to understand the infrastructure and technologies
supporting an AI-powered application.

A basic reconnaissance process can include:

```text
Target
  ↓
Port Discovery
  ↓
Service Discovery
  ↓
Technology Fingerprinting
  ↓
Identify AI-Related Components
  ↓
Map Attack Surface
  ↓
Threat Modelling
```

This connects directly with my existing experience using tools such as **Nmap** for network and service discovery.

---

## AI Threat Modelling Approach

The threat modelling concepts from this section helped me think about an **AI application as a complete architecture** rather than only focusing on the model.

A simplified approach is:

```text
Identify Assets
      ↓
Identify Components
      ↓
Identify Attack Surfaces
      ↓
Identify Threats
      ↓
Map Threats to Components
      ↓
Identify Security Controls
      ↓
Assess Remaining Risk
```

For AI systems, this process needs to account for additional areas such as models, training data, data supply chains, AI-specific components, user interaction, and supporting infrastructure.

---

## Practical Skills Developed

Through this section I developed practical understanding of:

* **OWASP Top 10 for LLM Applications**
* **MITRE ATLAS**
* **AI-specific attack surfaces**
* **LLM security threats**
* **Database, model, system, and user-based threats**
* **AI threat modelling**
* **Adapting traditional threat modelling concepts for AI**
* **AI system reconnaissance**
* **Port and service discovery**
* **Technology fingerprinting**
* **Mapping security risks to AI components**
* **Identifying appropriate security controls**
* **Applying AI security concepts through practical assessment**

---

## Connection to My Cybersecurity Background

This section connected strongly with the cybersecurity skills I have already developed.

My penetration testing experience with reconnaissance, service discovery, web application security, and attack-surface analysis provided a useful foundation for understanding AI system reconnaissance.

At the same time, AI threat modelling introduced a different perspective by requiring me to consider the complete AI ecosystem rather than only traditional infrastructure or web application vulnerabilities.

The combination of traditional cybersecurity knowledge with AI-specific frameworks such as OWASP LLM Top 10 and MITRE ATLAS is helping me build toward AI Security and AI Red Teaming.

---

## Key Takeaways

1. **AI Security Is System Security**  
   An AI model is only one component of a larger system. Security must also consider the surrounding infrastructure, applications, data, users, and supporting services.

2. **AI Introduces New Attack Surfaces**  
   AI-powered systems introduce additional components and dependencies that may not exist in traditional applications.

3. **Traditional Security Frameworks Still Matter**  
   Existing cybersecurity concepts such as reconnaissance and threat modelling remain valuable, but they need to be adapted to account for AI-specific risks.

4. **Frameworks Provide Structure**  
   OWASP LLM Top 10 and MITRE ATLAS provide useful ways to organize and understand AI security threats.

5. **Reconnaissance Is Still Fundamental**  
   Understanding exposed ports, services, technologies, and infrastructure is an important part of assessing an AI-powered system.

6. **Threat Modelling Helps Prioritize Risk**  
   Threat modelling provides a structured way to identify assets, attack surfaces, threats, and appropriate security controls before focusing on individual vulnerabilities.

---

## Reflection

This section was one of the most useful parts of my AI Security learning so far.

I particularly enjoyed the combination of traditional cybersecurity concepts with AI-specific security problems.

The areas that stood out most to me were LLM threat categories, AI threat modelling, OWASP LLM Top 10, MITRE ATLAS, and AI system reconnaissance.

The reconnaissance material was especially relevant to my penetration testing background because it showed how techniques such as port scanning and technology fingerprinting can be applied when assessing AI-powered systems.

The practical assessment at the end of the section also helped reinforce the concepts by requiring me to identify threats and appropriate security controls within an AI system architecture.

---

## Practical Assessment Result

### AI Threat Modelling Assessment

| Metric | Status |
| :--- | :--- |
| **Status** | ✅ Completed |
| **Score** | 100% |
| **Flags Captured** | 2/2 |
| **Assessment** | ✅ Passed |

---

## Status

**Completed — Section 02**

This section strengthened my understanding of AI-specific security frameworks, LLM threats, AI threat modelling, and AI system reconnaissance.

The knowledge from this section provides a foundation for progressing into more advanced AI Security, AI Red Teaming, and AI Defense topics.
