# AI Security Journey

> **Building on a cybersecurity foundation to specialize in securing AI systems.**

---

## About Me

I am a cybersecurity student focused on developing practical skills across
Security Operations, Penetration Testing, Web Application Security,
Vulnerability Research, and now AI Security.

My cybersecurity journey has been built around hands-on learning rather
than relying only on theoretical knowledge. I have developed experience
with security labs, SIEM technologies, networking, Linux, Windows security,
web application security, penetration testing, and vulnerability research.

I am now expanding this foundation into **AI Security**, with a focus on
understanding how AI systems work, how they can be attacked, and how they
can be secured.

---

## Why I Am Learning AI Security

Artificial Intelligence is becoming increasingly integrated into
software, businesses, security operations, and everyday technology.

As AI systems become more capable and widely deployed, securing these
systems is becoming an increasingly important cybersecurity challenge.

Rather than moving away from cybersecurity, I am building on the
cybersecurity foundation I already have and adding **AI Security as a
specialization**.

My goal is to understand the security of AI systems from both an
attacker's and defender's perspective.

I want to develop practical knowledge in areas such as:

- AI and Machine Learning fundamentals
- Large Language Models (LLMs)
- AI security threats
- AI models and data
- Prompt engineering and adversarial testing
- AI forensics
- AI application security
- AI red teaming
- AI-related vulnerabilities and attack techniques
- Defensive strategies and security controls
- AI supply-chain security
- Data poisoning and RAG security
- AI agent security

---

# Current Cybersecurity Foundation

Before starting my AI Security journey, I developed practical experience
across several areas of cybersecurity.

## Security Operations

- Completed the TryHackMe SOC Level 1 pathway
- Built a self-hosted Splunk SOC home lab
- Practiced security monitoring and log analysis
- Worked with Windows security events and SIEM concepts
- Created custom Splunk detections mapped to MITRE ATT&CK
- Practiced alert investigation and attack-chain reconstruction

## Web Security & Penetration Testing

- Completed the TryHackMe Web Fundamentals pathway
- Completed the TryHackMe Web Application Pentesting pathway
- Completed the TryHackMe Web Application Red Teaming pathway
- Completed the TryHackMe Junior Penetration Tester pathway
- Practiced reconnaissance and security testing
- Studied OWASP Top 10 concepts
- Practiced web application vulnerabilities in controlled environments
- Completed 30+ PortSwigger Web Security Academy labs covering areas such as SQL injection, broken access control, authentication flaws, and XSS

## Vulnerability Research

I have also started participating in real-world vulnerability research
through authorized vulnerability disclosure and bug bounty programs.

My research experience includes submissions to:

- HackerOne VDP programs
- Intigriti
- Bugcrowd
- Self-hosted authorized programs

These submissions have resulted in duplicate and informative classifications
as well as valuable triage feedback.

This experience has helped me improve my vulnerability validation,
impact assessment, research methodology, and security reporting.

## Practical Experience

I am also gaining practical cybersecurity experience through internships,
working on security research, security tooling, vulnerability analysis,
documentation, and hands-on cybersecurity projects.

---

# TryHackMe

TryHackMe has been a major part of my hands-on cybersecurity development.

I have completed **235+ hours of structured hands-on training** across
Security Operations, penetration testing, web application security,
web fundamentals, and AI Security.

I have also reached the **Top 1% globally** on TryHackMe, with
**296+ rooms completed**.

## Completed Learning Paths

- **SOC Level 1** — 65h 29m
- **Junior Penetration Tester** — 94h 25m
- **Web Application Pentesting** — 31h 53m
- **Web Application Red Teaming** — 25h 30m
- **Web Fundamentals** — 20h 50m
- **AI Security** — Completed

The AI Security pathway became the foundation for this repository and
expanded my learning into practical AI security concepts and attacks.

---

# AI Security Learning Journey

This repository documents my ongoing journey into AI Security through
structured learning, practical challenges, security research, and
independent projects.

A major part of this journey has been the **TryHackMe AI Security**
pathway.

The pathway introduced practical concepts across:

- AI fundamentals
- AI security
- Prompt security
- AI supply-chain security
- Data poisoning
- LLM security
- Prompt injection
- Jailbreaking
- AI model manipulation
- RAG security
- Sensitive information disclosure
- AI security defenses

The complete pathway has now been completed.

---

# TryHackMe AI Security Pathway

## Section 01 — AI Fundamentals

**Status: ✅ Completed**

This section established the foundation for understanding modern AI
systems and the technologies behind them.

Topics covered included:

- Artificial Intelligence fundamentals
- Machine Learning concepts
- AI models
- How modern AI systems operate
- Security considerations surrounding AI technologies

Documentation:

`TryHackMe-AI-Security/Section-01-AI-Fundamentals/`

---

## Section 02 — AI Security

**Status: ✅ Completed**

This section introduced the security risks associated with AI systems
and established the foundation for approaching AI from an offensive and
defensive security perspective.

Topics covered included:

- AI security threats
- AI attack surfaces
- Security risks involving AI systems
- AI-specific attack techniques
- Defensive considerations

Documentation:

`TryHackMe-AI-Security/Section-02-AI-Security/`

---

## Section 03 — Prompt Security

**Status: ✅ Completed**

This section focused on the security of prompts and interactions with
Large Language Models.

Topics included:

- Prompt Injection
- Jailbreaking
- Prompt Defense
- Instruction manipulation
- Model behavior manipulation
- Adversarial prompting
- Defensive approaches to prompt-based attacks

### Practical CTFs

#### LLMborghini

A practical AI security challenge focused on **indirect prompt injection**.

I tested ways to manipulate the model through indirect instructions,
including attempting to make the model disclose information that it was
not originally intended to reveal.

After observing the model's behavior, I used the disclosed information
to identify where the flag could be obtained and successfully retrieved it.

#### White Rabbit

A second prompt-injection-focused challenge involving model manipulation.

I tested instruction overriding techniques against the model and
successfully manipulated the model to reveal the challenge flags.

Documentation:

`TryHackMe-AI-Security/Section-03-Prompt-Security/`

---

## Section 04 — AI Supply Chain Security

**Status: ✅ Completed**

This section focused on the security risks introduced through the
components and dependencies used by AI systems.

Topics included:

- AI supply chains
- Model artifacts
- External models
- Datasets
- Packages and dependencies
- Supply-chain attack vectors
- Securing AI supply chains
- Model inspection
- Dependency auditing
- Supply-chain governance

### Practical Challenges

The section also included practical security scenarios involving
compromised or potentially malicious AI components and required
investigation of the resulting security issues.

Documentation:

`TryHackMe-AI-Security/Section-04-AI-Supply-Chain-Security/`

---

## Section 05 — Data Poisoning

**Status: ✅ Completed**

The final section focused on **data poisoning and RAG security**.

The section covered:

- RAG Security Fundamentals
- Data Poisoning in RAG Systems
- Sensitive Information Disclosure
- AI assistant security
- Retrieval manipulation
- Data integrity
- Trust boundaries
- Sensitive data exposure
- AI model manipulation

### Practical CTFs

#### UnIndexed

A practical AI security challenge involving an AI assistant with access
to a large amount of information.

I investigated the model's capabilities through a sequence of prompts.

The interaction included:

1. Asking what the model could do.
2. Investigating the ATLAS project mentioned by the model.
3. Asking whether the project contained hidden information or secrets.

Through this model-manipulation approach, the model disclosed the flag.

This challenge demonstrated how conversational context and carefully
constructed questions can be used to extract information that should not
be exposed by an AI assistant.

#### Lockdown

A practical AI security challenge involving an AI assistant with
multiple vulnerabilities.

The objective was to identify the weaknesses, understand how the model
could be manipulated, and demonstrate the resulting security impact.

The challenge reinforced the importance of securing AI assistants
against model manipulation and unintended information disclosure.

Documentation:

`TryHackMe-AI-Security/Section-05-Data-Poisoning/`

---

# TryHackMe AI Security Certificate

The **TryHackMe AI Security pathway has been completed**, and the
certificate of completion is included in this repository as supporting
evidence.

The certificate documents completion of the structured AI Security
learning path.

---

# AI Security Projects

The repository also contains independent projects created to move beyond
structured learning and apply AI security concepts in practical
environments.

## Prompt Lab

An independent interactive security learning project focused on
understanding prompt-based attacks and defensive concepts.

The project explores concepts such as:

- Prompt injection
- Instruction hierarchy
- Adversarial prompts
- Prompt manipulation
- Security awareness
- Defensive prompt design

The project is maintained separately while this repository documents its
role in my broader AI Security journey.

---

## Prompt Injection Defense Lab

An independent browser-based AI Security project focused specifically on
understanding and defending against prompt injection attacks.

The project was designed to turn prompt-injection concepts into an
interactive learning and experimentation environment.

Topics include:

- System vs user instructions
- Instruction hierarchy
- Direct prompt injection
- Indirect prompt injection
- Role and instruction hijacking
- Delimiter attacks
- Context manipulation
- Data-exfiltration attempts
- Conflicting instructions
- Defensive system prompts
- Output constraints
- Least privilege
- Separating instructions from untrusted data

The project includes interactive exercises, simulated AI responses,
heuristic feedback, before/after comparisons, and local progress
tracking.

Documentation:

`Projects/Prompt-Injection-Defense-Lab/`

## RAG Security Lab

An independent interactive security learning project focused on understanding Retrieval-Augmented Generation (RAG) attacks and layered defensive concepts.

The project explores concepts such as:

- Data poisoning
- Retrieval manipulation
- Indirect prompt injection
- Sensitive information disclosure
- Chunk trust scoring
- Instruction hierarchy
- Output filtering
- Defense-in-depth
---

# Documentation Philosophy

This repository documents my **overall AI Security learning journey**
across different platforms, training programs, practical exercises,
research, and projects.

The goal is not to document every individual learning activity.

Instead, I focus on work that demonstrates meaningful understanding and
practical application.

I prioritize documenting:

- Important concepts and security techniques
- Section-level or module-level learning
- Practical challenges and exercises
- AI Security research
- Attack and defense techniques
- Hands-on experiments
- Screenshots and supporting evidence
- Lessons learned and personal observations
- Security assessments and findings
- CTF challenges
- Capstone projects
- Independent AI Security projects

The goal is to demonstrate:

**What I learned → What I practiced → What I discovered → How I applied it**

---

# Repository Structure

```text
ai-security-journey/
│
├── README.md
│
├── TryHackMe-AI-Security/
│   │
│   ├── Section-01-AI-Fundamentals/
│   │   └── README.md
│   │
│   ├── Section-02-AI-Security/
│   │   └── README.md
│   │
│   ├── Section-03-Prompt-Security/
│   │   └── README.md
│   │
│   ├── Section-04-AI-Supply-Chain-Security/
│   │   └── README.md
│   │
│   └── Section-05-Data-Poisoning/
│       └── README.md
│
├── Other-Learning/
│   └── InfoSecLabs-AI-Security/
|   ├── README.md
|   └── InfoSecLabs-AI-Security-The-New-Frontier.pdf
|
└── Projects/
    ├── Prompt-Lab/
    │   └── README.md
    │
    ├── Prompt-Injection-Defense-Lab/
    │   └── README.md
    │
    └── RAG-Security-Lab/
        └── README.md
```

## Structure Overview

```text
TryHackMe-AI-Security/
├── Contains documentation from the completed TryHackMe AI Security pathway, organized by its five major sections.
│
Other-Learning/
├── Contains AI Security learning from other platforms, courses, certifications, labs, research programs, and structured training outside TryHackMe.
│   └── InfoSecLabs-AI-Security/
│       └── Documents my completed InfoSecLabs "AI Security (The New Frontier)" learning path and credential.
│
Projects/
├── Contains independent AI Security projects that demonstrate practical application beyond individual learning platforms.
│   ├── Prompt-Lab/
│   │   └── Documents my independent Prompt Lab project.
│   │
│   ├── Prompt-Injection-Defense-Lab/
│   │   └── Documents my independent project focused on understanding and defending against prompt injection attacks.
│   │
│   └── RAG-Security-Lab/
│       └── Documents my independent project exploring RAG-specific attacks and layered defenses.
```

## Progress

| Area | Status |
| :--- | :--- |
| **TryHackMe AI Security — Section 01: AI Fundamentals** | ✅ Completed |
| **TryHackMe AI Security — Section 02: AI Security** | ✅ Completed |
| **TryHackMe AI Security — Section 03: Prompt Security** | ✅ Completed |
| **TryHackMe AI Security — Section 04: AI Supply Chain Security** | ✅ Completed |
| **TryHackMe AI Security — Section 05: Data Poisoning** | ✅ Completed |
| **TryHackMe AI Security Pathway** | ✅ Completed |
| **TryHackMe AI Security Certificate** | ✅ Added |
| **Prompt Lab** | ✅ Completed |
| **Prompt Injection Defense Lab** | ✅ Completed |
| **RAG Security Lab** | ✅ Completed |
| **Other AI Security Learning** | 🔄 Ongoing |
| **AI Security Research** | 🔄 Ongoing |
| **AI Security Projects** | 🔄 Ongoing |

## Skills Developed

Through this journey, I have developed practical exposure to:

### 🛡️ AI Security
* AI security fundamentals
* LLM security
* AI attack surfaces
* AI threat modeling
* AI security testing

### ⚡ Prompt Security
* Prompt injection
* Indirect prompt injection
* Jailbreaking
* Instruction hijacking
* Model manipulation
* Prompt defense

### 📊 AI Data Security
* Data poisoning
* RAG security
* Retrieval manipulation
* Sensitive information disclosure
* Data integrity
* Trust boundaries

### 📦 AI Supply Chain Security
* Model artifacts
* External dependencies
* AI packages
* Supply-chain attack vectors
* Dependency security
* Model and dependency auditing

### 🧪 Practical Security
* Adversarial testing
* CTF-based security research
* Security experimentation
* Vulnerability analysis
* Security documentation
* Controlled security testing

---

## Goals

My goals for this journey are to:

* Build a strong foundation in AI Security
* Understand common AI attack surfaces
* Learn offensive AI security and red teaming
* Understand defensive AI security practices
* Apply cybersecurity knowledge to AI systems
* Complete practical AI security challenges
* Build meaningful AI Security portfolio projects
* Research emerging AI security vulnerabilities
* Develop practical AI red-teaming skills
* Explore AI application and agent security
* Develop skills that can support a future transition into an AI Security role

---

## Long-Term Direction

My long-term goal is to combine my cybersecurity background with AI Security rather than treating them as separate fields.

```text
Cybersecurity Foundation
├── Security Operations
├── Penetration Testing
├── Web Application Security
├── Vulnerability Research
├── Threat Detection
└── Network Security
        ↓
AI Security Specialization
├── AI Application Security
├── LLM Security
├── AI Red Teaming
├── AI Threat Detection
├── AI/Agent Security
├── AI Vulnerability Research
├── AI Supply Chain Security
└── AI Data Security
        ↓
Goal
Become a cybersecurity professional capable of securing modern AI-powered systems.
```

## Disclaimer

This repository contains my personal learning notes, practical work, observations, CTF solutions, and projects created during my AI Security learning journey.

All security testing documented here is performed in authorized labs, controlled environments, intentionally vulnerable applications, or programs where I have permission to test.

No unauthorized security testing is intended or documented.

---

## What's Next?

Completing the TryHackMe AI Security pathway is not the end of the journey.

The next phase will focus on turning the concepts learned into deeper practical experience through:

* AI red teaming
* LLM application security
* AI agent security
* RAG security testing
* AI threat modeling
* Prompt injection research
* AI vulnerability research
* AI security tooling
* Independent security labs
* Portfolio projects
* Responsible vulnerability research

The objective is to move from learning AI Security toward **actively testing, researching, and building secure AI systems.**

---

## Journey Philosophy

$$\text{Learn} \longrightarrow \text{Practice} \longrightarrow \text{Break} \longrightarrow \text{Understand} \longrightarrow \text{Defend} \longrightarrow \text{Build} \longrightarrow \text{Document}$$

---

## About

My practical journey into AI Security — documenting hands-on learning, security challenges, research, projects, and practical experimentation.
