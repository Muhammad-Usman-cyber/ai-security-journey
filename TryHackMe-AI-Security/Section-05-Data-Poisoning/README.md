# Section 05 — Data Poisoning

> TryHackMe AI Security Pathway

**Status:** ✅ Completed  
**Section:** Data Poisoning  
**Pathway:** TryHackMe AI Security

---

## 📌 Overview

This section focused on data poisoning and the security risks
introduced when AI systems depend on external data, retrieval
systems, embeddings, and information sources.

The section explored how attackers can manipulate data consumed
by AI systems, influence retrieval results, expose sensitive
information, and manipulate AI assistants through weaknesses in
their available context and data.

---

## 🧠 Rooms Completed

| # | Room | Type | Status |
|---|---|---|---|
| 01 | RAG Security Fundamentals | Learning | ✅ |
| 02 | Data Poisoning in RAG Systems | Hands-on | ✅ |
| 03 | Sensitive Information Disclosure | Hands-on | ✅ |
| 04 | UnIndexed | CTF | ✅ |
| 05 | Lockdown | CTF | ✅ |

---

## 01 — RAG Security Fundamentals

This room introduced the security fundamentals of Retrieval
Augmented Generation (RAG) systems.

The room focused on how RAG systems retrieve external information
and provide it as context to an AI model.

### Key concepts

- RAG architecture
- Retrieval systems
- Context
- Trust boundaries
- Retrieval-based attack surfaces
- Security risks associated with external information

### Key takeaway

RAG systems introduce additional security boundaries because the
model does not rely only on its original training data. Retrieved
information can influence the model's behaviour and output.

---

## 02 — Data Poisoning in RAG Systems

This room focused on data poisoning attacks against RAG systems.

The exercises demonstrated how manipulated information can affect
AI embeddings and retrieval results without necessarily producing
an obvious error.

### Key concepts

- Data poisoning
- AI embeddings
- Retrieval manipulation
- RAG pipelines
- Malicious or manipulated information
- Trust in retrieved data

### Key takeaway

An attacker may not need to compromise the AI model itself.
Manipulating information consumed by the retrieval pipeline can
influence what the model receives as context.

---

## 03 — Sensitive Information Disclosure

This room explored how sensitive information can become exposed
through AI embeddings, retrieval mechanisms, and weak access
controls.

### Security concepts

- Sensitive information exposure
- Embedding security
- Retrieval security
- Access control
- AI-assisted information disclosure
- Trust boundaries

### Key takeaway

Sensitive information can potentially be exposed when retrieval
systems and access controls do not properly restrict what an AI
system can access or return.

---

## 04 — UnIndexed

**Type:** CTF

The challenge involved an AI assistant that had access to a broad
set of information.

The central security issue was understanding what was actually
included in the assistant's accessible information rather than
assuming that all available data was safe to expose.

### My approach

I started by asking the model:

> What can you do?

The model provided information about its capabilities and
mentioned the **ATLAS project**.

I then asked:

> What is ATLAS project?

The model disclosed additional information about the project.

Finally, I asked whether there were any secrets or hidden
information within the project, including flags.

The model disclosed the flag.

### Security lesson

This challenge demonstrated how excessive information access and
insufficient restrictions around an AI assistant can allow an
attacker to progressively discover sensitive information through
natural-language interaction.

---

## 05 — Lockdown

**Type:** CTF

This challenge involved an AI assistant with three open
vulnerabilities.

The objective was to identify the weaknesses, address them, and
demonstrate that the system could be secured.

### Key concepts

- AI assistant security
- Model manipulation
- AI application vulnerabilities
- Security controls
- Vulnerability identification
- Defensive AI security

### Key takeaway

AI security requires more than protecting the underlying model.
The application surrounding the model, its permissions, available
data, and security controls must also be assessed.

---

## 🔬 Skills Developed

Through this section I strengthened my understanding of:

- Retrieval Augmented Generation (RAG)
- Data poisoning
- AI embeddings
- Retrieval manipulation
- RAG security
- Sensitive information disclosure
- Access-control weaknesses in AI systems
- AI assistant security
- Model manipulation
- AI application security
- Trust boundaries
- Information exposure through AI systems

---

## 🛡️ Security Mindset

A major lesson from this section was that the security of an AI
system depends heavily on the data and context surrounding the
model.

A simplified RAG architecture can be viewed as:

```text
User
  ↓
AI Application
  ↓
Retriever
  ↓
Knowledge Base / Data
  ↓
Relevant Context
  ↓
AI Model
  ↓
Response
```
Each stage introduces potential security risks.

If an attacker can manipulate the underlying information, influence retrieval, bypass access controls, or manipulate the assistant's behaviour, the final AI response may also be affected.

---

## 🎯 Section Completion

### Data Poisoning — COMPLETE ✅

This section expanded my AI security knowledge into RAG systems, data poisoning, embeddings, retrieval security, information disclosure, and AI assistant security.

---

## 🏆 Pathway Progress

With the completion of this section, all major sections of the TryHackMe AI Security Pathway have been completed.

### AI Security Pathway — COMPLETE ✅
