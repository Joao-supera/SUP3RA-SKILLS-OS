🟦 BLOCO 1: ARQUIVOS DA RAIZ (4 arquivos)
1. Nome do arquivo: ARCHITECTURE.md

# SUP3RA Skills OS Architecture

SUP3RA Skills OS is a modular architecture for building AI agents with reusable skills, governance, memory, context and human review.

The goal is not to create uncontrolled autonomous agents.
The goal is to create AI systems that can:
- understand context;
- select the right skill;
- respect operational limits;
- support human decisions;
- use business knowledge;
- generate auditable outputs;
- improve through feedback.

## Core Thesis

> Prompt is instruction.  
> Skill is capability.  
> System is advantage.

A prompt tells an AI what to do once.
A skill gives an agent a reusable capability.
A system connects skills, memory, tools, context, governance and feedback into a reliable workflow.

## High-Level Flow

```mermaid
flowchart TD
    A[User Input] --> B[CORE Constitution]
    B --> C[Trust Core]
    C --> D[Skill Selection]
    D --> E[Agent Execution]
    E --> F{Risk Level}
    F -->|Low| G[Direct Output]
    F -->|Medium| H[Output with Assumptions and Limits]
    F -->|High| I[Human Review Required]
    F -->|Critical| J[Safe Refusal or Safe Alternative]
    G --> K[Feedback]
    H --> K
    I --> K
    J --> K
    K --> L[Memory / Learning Update]

    Main Layers
1. Input Layer
Receives user messages, business context, documents, forms, process descriptions, customer feedback, and operational data.
2. CORE Constitution
Defines non-negotiable rules. Prevents hallucinated certainty, manipulation, unsafe automation, hidden assumptions, privacy violations, and high-impact decisions without review.
3. Trust Core
Evaluates risk level, sensitive data, uncertainty, source reliability, need for human review, auditability, and safe response boundaries.
4. Skill Selection
Chooses the most relevant reusable capability (Diagnostic, Decision, Content, Agent Builder, Governance, Business Ops, Monte Carlo).
5. Agent Execution
Selected agents apply one or more skills to produce an output (Lead Management, Content, Decision, Governance, Customer Support).
6. Human Review Gate
Required when output may affect rights, money, health, legal exposure, hiring, reputation, sensitive personal data, or irreversible business decisions.
7. Memory and Feedback
Stores useful context, decisions made, user preferences, process rules, common failures, and lessons learned. Respects privacy, consent, and data minimization.
Design Principle
Do not build one giant prompt. Build a system where each skill has:
a purpose;
activation conditions;
inputs;
process;
output format;
safety rules;
examples;
success metric.
Final Principle
A prompt generates a response.
A skill creates a capability.
A system creates continuity.


#### 2. Nome do arquivo: `GOVERNANCE.md`
```markdown
# SUP3RA Skills OS Governance

Governance is the layer that makes AI systems safer, more transparent and more useful in real business environments.

SUP3RA Skills OS is designed around one principle:
> AI should support human judgment, not replace it.

## Governance Goals
- reduce hallucinations;
- protect sensitive data;
- preserve human autonomy;
- prevent unsafe automation;
- make uncertainty visible;
- require human review when needed;
- create auditability;
- improve trust through clear limits.

## Core Rules
The system must not:
- invent facts;
- hide uncertainty;
- present assumptions as facts;
- manipulate users;
- create false urgency;
- promise guaranteed results;
- expose sensitive data;
- make high-impact decisions without human review;
- pretend to be a human, legal authority, doctor, therapist or financial advisor.

## Risk Levels

### Low Risk
Examples: general content, simple brainstorming, formatting, low-impact explanations.
Action: respond directly.

### Medium Risk
Examples: business communication, customer-facing drafts, operational recommendations, internal workflow suggestions.
Action: respond with assumptions, limits and recommended review when relevant.

### High Risk
Examples: legal, financial, medical or hiring-related topics; customer complaints; reputational risk; sensitive data; important business decisions.
Action: require human review before execution.

### Critical Risk
Examples: illegal requests, harmful actions, deception, manipulation, unsafe automation, privacy violations.
Action: refuse unsafe execution and provide a safe alternative.

## Human Review Required
When task involves: legal impact, medical impact, financial risk, hiring/firing, sensitive personal data, automated rejection, compliance, reputation, irreversible decisions, or high uncertainty with high consequences.

## Required Distinctions
Outputs should separate: fact, inference, hypothesis, estimate, recommendation, limitation, next step.

## Audit Log Format
Use this structure for traceable decisions:
```text
Request:
Context:
Skill used:
Risk level:
Sensitive data involved:
Sources or basis:
Assumptions:
Limitations:
Human review needed:
Recommended action:
Output summary:

Data Protection Principles
Data minimization, purpose limitation, access control, retention limits, masking of sensitive data, secure storage, human oversight for sensitive workflows, clear policies for AI processing boundaries.
Final Principle
Trust is not created by confident answers.
Trust is created by visible limits, clear rules, human oversight and accountable execution.


#### 3. Nome do arquivo: `ROADMAP.md`
```markdown
# SUP3RA Skills OS Roadmap

This roadmap describes the evolution from public framework to applied agent system.

## Phase 1 — Public Framework (Current)
Goal: create a clear public architecture.
Deliverables: README, ARCHITECTURE, GOVERNANCE, skill-template, diagnostic-skill, decision-skill, content-skill, trust-core-skill, small-business-diagnostic.
Success metric: repository clearly communicates thesis, architecture and practical use cases.

## Phase 2 — Skill Library
Goal: expand library of reusable agent skills.
Planned skills: Agent Builder, Business Ops, Lead Management, RAG Knowledge Base, Design Identity, Memory, Monte Carlo, Customer Support, Sales Follow-up.
Success metric: each skill has purpose, inputs, process, output format, safety rules and example.

## Phase 3 — Agent Cards
Goal: create applied agents using combinations of skills.
Planned agents: Lead Management, Content, Decision, Governance, Customer Support, Sales Follow-up, Small Business Diagnostic.
Success metric: each agent card explains function, required skills, restrictions and human review triggers.

## Phase 4 — Examples and Blueprints
Goal: demonstrate real-world use cases.
Planned examples: AI lead management system, WhatsApp follow-up workflow, Small business AI diagnosis, Content strategy assistant, Decision support workflow, Governance checklist.
Success metric: recruiter/client/developer can understand application to real business scenarios.

## Phase 5 — MVP Prototype
Goal: transform framework into functional prototype.
Stack: Next.js, React, Tailwind CSS, Supabase, OpenAI/compatible LLM, Vector DB, GitHub-based skill repo, Basic dashboard, Human review queue.
Features: upload business context, run diagnostic skill, recommend agents, generate action plan, classify risk, require human review, export report.

## Phase 6 — SaaS Evolution
Goal: evolve into SUP3RA Skills OS product.
Features: skill manager, agent builder, knowledge base, governance dashboard, decision logs, audit trail, team workspace, RAG integration, business process templates, memory/feedback loop.

## Strategic Direction
Long-term goal: help businesses move from isolated AI prompts to governed systems of reusable agent capabilities.
> From prompts to skills.
> From skills to systems.
> From systems to better decisions.

