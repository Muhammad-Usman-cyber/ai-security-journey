# RAG Security Lab

An interactive AI security lab built through iterative AI-assisted development.

RAG Security Lab teaches Retrieval-Augmented Generation attacks and defenses through hands-on practice with a real TF-IDF retrieval pipeline. Users toggle attacks (data poisoning, retrieval manipulation, indirect prompt injection, sensitive information disclosure), toggle defenses, and observe — in a real, non-scripted pipeline — what actually gets through.

## Key Features

- Real, live TF-IDF retrieval and cosine similarity — not scripted results
- 4 attacks and 4 defenses, each with an honest stated residual risk
- Defense-effectiveness metric and live attack status (blocked/succeeded)
- 3 pre-built scenarios mapped to the OWASP LLM Top 10
- Fully client-side, no API key required

## Why It Matters to My AI Security Journey

This project extends my prompt injection work into RAG-specific attack surface — data poisoning, retrieval manipulation, and indirect injection via retrieved documents. It reinforced the central lesson that no single defense fully secures a RAG pipeline; layered, complementary controls are required.

## Links

* [Live Demo](https://muhammad-usman-cyber.github.io/rag-security-lab/)
* [Project Repository](https://github.com/Muhammad-Usman-cyber/rag-security-lab)
