# Agent Builder Skill

## Purpose
Transforms a business need into a specialized AI agent design. Defines what the agent should do, required skills, allowed data, restrictions and human review points.

## When to Use
Creating customer support, lead management, content, sales, decision support, governance agents, internal assistants, automation copilots, business workflow agents.

## Inputs
Business context, User goal, Target users, Main tasks, Required data, Tools/systems involved, Risk level, Human review points, Success metric, Output format.

## Agent Design Framework
Agent Name:
Purpose:
Target User:
Main Tasks:
Required Skills:
Allowed Data:
Restricted Data:
Tools:
Human Review Required When:
Risks:
Output Format:
Success Metrics:

## Required Skills
Diagnostic, Decision, Content, Trust Core, Business Ops, RAG, Memory, Monte Carlo.

## Safety Rules
Must not: invent facts, act outside scope, use sensitive data without permission, make high-impact decisions alone, bypass human review, promise guaranteed outcomes, hide uncertainty, automate unsafe workflows.

## Example
Agent Name: Lead Management Agent
Purpose: Organize incoming leads, classify intent and suggest next commercial actions.
Target User: Small business owner or sales team.
Main Tasks: classify lead intent, summarize messages, detect urgency, suggest response, recommend follow-up, update CRM/spreadsheet.
Required Skills: Diagnostic, Business Ops, Trust Core, Content.
Allowed Data: Lead message, channel, service interest, interaction history.
Restricted Data: Sensitive personal data, payment data, legal/medical info unless explicitly required.
Human Review Required When: sensitive complaint, legal/financial/medical advice request, discount/contract terms, liability risk.
Risks: Wrong classification, unsupported promises, data exposure.
Output Format: Lead summary, intent, urgency, suggested reply, next action, risk flag.
Success Metrics: First response time, handoff rate, lead follow-up completion, classification accuracy.

## Final Principle
A good agent is not defined by how much it can do. It is defined by what it can do reliably, safely and repeatedly.
