# Section 3 — Prompt Security

## TryHackMe AI Security Pathway

This section focuses on security risks involving prompts and
Large Language Models (LLMs), including prompt injection,
jailbreaking, and defensive techniques.

## Rooms Completed

### 1. Prompt Injection
Learned how malicious or carefully crafted instructions can
manipulate an AI system into ignoring or conflicting with its
intended instructions.

Key concepts:
- Direct prompt injection
- Indirect prompt injection
- Instruction manipulation
- Instruction hierarchy
- Untrusted content influencing model behavior
- Data disclosure through manipulated model responses

### 2. Jailbreaking
Explored techniques designed to bypass an AI model's intended
restrictions and safety behavior.

Key concepts:
- Safety restriction bypass attempts
- Role/instruction manipulation
- Conflicting instructions
- Adversarial prompting
- Model behavior under manipulated context

### 3. Prompt Defense
Studied defensive approaches for reducing prompt-based attacks.

Key concepts:
- Separating trusted instructions from untrusted data
- Strong system instructions
- Input validation
- Output constraints
- Least-privilege principles
- Limiting sensitive information available to the model
- Treating external content as untrusted

---

# CTFs Completed

## LLMborghini

### Objective

Put indirect prompt injection skills to the test in an AI
security challenge.

### Approach

I investigated how the model responded to manipulated or
untrusted instructions.

I was able to influence the model into revealing information
that it was not supposed to expose. After identifying the
information-disclosure behavior, I focused on the question
containing the flag and applied the same technique to obtain
the flag.

### Key Learning

The challenge demonstrated how indirect prompt injection can
cause an AI system to follow instructions contained in
untrusted context instead of maintaining the intended
instruction boundaries.

---

## White Rabbit

### Objective

Test prompt injection techniques against another AI-based
challenge.

### Approach

I used prompt manipulation to override the model's intended
behavior and successfully obtained all three flags.

### Key Learning

The challenge reinforced how instruction hierarchy and
untrusted input can be abused when an AI system does not
properly distinguish trusted instructions from attacker-
controlled content.

---

# Key Takeaways

- Prompt injection can manipulate an AI model through crafted
  instructions or untrusted content.
- Indirect prompt injection is particularly important when an
  application processes external content.
- Jailbreaking attempts to bypass intended model restrictions.
- AI systems should not blindly trust instructions contained
  within user-controlled or external data.
- Defensive prompt design should be combined with application-
  level controls such as validation, access control, and
  least-privilege design.

## Status

✅ Section 3 — Completed
