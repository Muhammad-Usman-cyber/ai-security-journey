# Section 04 — AI Supply Chain Security

> TryHackMe AI Security Pathway

**Status:** ✅ Completed  
**Focus:** AI/ML Supply Chain Security

---

## 📌 Overview

This section focused on the security risks introduced by the
AI supply chain — from models and datasets to dependencies,
repositories, APIs, and deployment pipelines.

The main objective was to understand how attackers can compromise
trusted AI components and how defenders can identify, verify, and
secure those components before they reach production.

The section progressed from understanding the AI supply chain,
to investigating attack vectors, and finally to implementing
defensive controls and evaluating suspicious AI components.

---

## 🧠 Rooms Completed

| # | Room | Type | Status |
|---|---|---|---|
| 01 | Understanding AI Supply Chains | Learning | ✅ Completed |
| 02 | Supply Chain Attack Vectors | Learning / Hands-on | ✅ Completed |
| 03 | Securing the AI Supply Chain | Defensive / Hands-on | ✅ Completed |
| 04 | Payload | CTF | ✅ Completed |
| 05 | Checkpoint | CTF | ✅ Completed |

---

# 01 — Understanding AI Supply Chains

### What I learned

This room introduced the AI supply chain and how it differs
from a traditional software supply chain.

Key areas included:

- AI models
- Datasets
- ML frameworks
- Dependencies
- Model repositories
- Infrastructure
- AI APIs
- Trust relationships between supply-chain components

I also learned that AI supply-chain attacks can target multiple
layers rather than only the application using the model.

### Key takeaway

A model that appears trustworthy can still introduce security
risks if its origin, integrity, dependencies, or behaviour have
not been properly verified.

### Frameworks covered

- OWASP LLM03 — Supply Chain Vulnerabilities
- MITRE ATLAS — AML.T0010 ML Supply Chain Compromise

---

# 02 — Supply Chain Attack Vectors

This room moved from theory into practical investigation of
AI supply-chain attacks.

### Attack vectors studied

- Malicious model serialization
- Dependency confusion
- Typosquatting
- Model repository manipulation
- Compromised model artifacts
- API provider compromise
- Prompt template compromise

### Practical security concepts

I investigated how malicious model files can potentially execute
code during loading and learned why model files should not
automatically be treated as trusted data.

The room also introduced the importance of safely analysing
suspicious model artifacts instead of loading them directly.

### Key takeaway

The AI supply chain can be attacked at several different
trust boundaries.

Securing only the final AI application is not enough.

---

# 03 — Securing the AI Supply Chain

This room focused on defensive controls for AI/ML supply chains.

### Defensive techniques learned

- SafeTensors
- `weights_only=True`
- SHA-256 integrity verification
- Model provenance verification
- Model card review
- Fickling
- ModelScan
- Dependency auditing
- `pip-audit`
- Software Bills of Materials (SBOMs)
- Syft
- Architecture-level inspection
- API provider assessment
- Behaviour monitoring

### SupplySecLab

A major part of the room involved understanding the idea of
building a dedicated supply-chain security testing environment.

The goal is to identify malicious or suspicious components
before they enter production.

### Key takeaway

AI supply-chain security requires verification rather than
blind trust.

Model provenance, integrity, static analysis, dependency
security, architecture inspection, and behavioural monitoring
all contribute to reducing supply-chain risk.

---

# 04 — Payload

### Type

CTF / Incident Investigation

### Scenario

The challenge involved investigating a production AI code-review
model that was unexpectedly communicating externally.

The objective was to investigate the breach and determine how
the malicious model had been introduced into the environment.

### Skills reinforced

- AI/ML supply-chain incident investigation
- Model artifact analysis
- Suspicious outbound communication analysis
- Model provenance investigation
- Static analysis of serialized model files
- Identifying malicious model behaviour
- Investigating a compromised replacement artifact

The challenge reinforced an important concept:

> A compromised AI model can become an attack vector against the
> infrastructure running it.

---

# 05 — Checkpoint

### Type

CTF / Security Assessment

### Scenario

The challenge presented four code-review model candidates that
had undergone evaluation.

The task was to assess the evidence and investigate the suspicious
candidate before making a production decision.

### Investigation areas

- Model loading telemetry
- Suspicious file access
- Security guardrail configuration
- Policy templates
- Model provenance
- Supply-chain relationships
- Behavioural evidence
- Production security assessment

The challenge required connecting evidence across different
artifacts rather than relying on a single indicator.

### Key takeaway

AI supply-chain security is not simply about checking whether a
model works.

Security teams need to evaluate:

- Where the model came from
- What it contains
- What it accesses
- What dependencies it uses
- What controls are enabled
- Whether its behaviour matches expectations
- Whether its provenance can be verified

---

# 🔬 Practical Skills Developed

Through this section I strengthened my understanding of:

- AI/ML supply-chain threats
- Malicious model artifacts
- Model serialization risks
- Dependency confusion
- Repository attacks
- Model provenance
- Integrity verification
- Static model analysis
- Behavioural analysis
- Dependency auditing
- SBOM concepts
- AI API security
- Supply-chain incident investigation
- Production model assessment

---

# 🛡️ Security Mindset

The biggest lesson from this section was that AI security
extends beyond the model itself.

An AI system depends on an ecosystem of:

```text
Models
   ↓
Datasets
   ↓
Frameworks
   ↓
Dependencies
   ↓
Repositories
   ↓
APIs
   ↓
Infrastructure
   ↓
Production
```

Every trust relationship in that chain can introduce an attack surface.

Therefore, AI security requires verification and monitoring throughout the lifecycle rather than trusting a component simply because it appears legitimate.

---

## 📚 TryHackMe Resources

* **AI Supply Chain Security Module**
  * Understanding AI Supply Chains
  * Supply Chain Attack Vectors
  * Securing the AI Supply Chain
  * Payload Checkpoint

---

## 🎯 Completion

### Section 04 — AI Supply Chain Security: COMPLETE ✅

This section expanded my AI security journey from prompt-level attacks into the broader security of the models, dependencies, artifacts, APIs, and infrastructure that AI systems rely on.
