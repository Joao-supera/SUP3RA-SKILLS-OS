# Skill Name

## Purpose
Explain what this skill helps the agent do.

## When to Use
Use this skill when:
- condition 1;
- condition 2;
- condition 3.

## Inputs
The agent needs:
1. Input 1
2. Input 2
3. Input 3

## Process
The agent should:
1. Step one
2. Step two
3. Step three

## Output Format
```text
Section 1:
Section 2:
Section 3:
Next Step:

Safety Rules
The agent must not:
invent data;
overstate certainty;
manipulate;
automate sensitive decisions without review.
Example
User: Example request.
Agent output: Example response.
Success Metric
This skill is successful when:
the output is clear;
the user can act;
the risk is visible;
the next step is measurable.
Final Principle
One skill. One clear capability. One practical outcome.


---

### 🟩 BLOCO 2: SKILLS (5 arquivos)

#### 5. Nome do arquivo: `skills/diagnostic-skill.md`
*(Crie a pasta `skills` digitando o nome completo)*
```markdown
# Diagnostic Skill

## Purpose
Helps an AI agent understand a business, identify bottlenecks, map repetitive tasks and detect where AI can generate practical value. Designed to clarify, not to impress.

## When to Use
Business problems, operational bottlenecks, inefficient processes, lost leads, repetitive tasks, unclear priorities, AI opportunities, automation potential, decision-making gaps.

## Inputs
Ask or infer:
1. What does the business do?
2. Who is the customer?
3. What is the main objective?
4. What is working well vs. what is not?
5. Where is time being wasted?
6. Where are leads/opportunities being lost?
7. What tasks repeat every week?
8. What tools are currently used?
9. What decision needs improvement?

## Output Format
1. Diagnosis Summary
2. Main Bottleneck
3. Root Cause Hypothesis
4. AI Opportunity
5. Recommended First Agent
6. Risk
7. Next Step
8. Success Metric

## Diagnostic Logic
Separate: declared problem, probable real problem, symptoms, root causes, constraints, opportunities, risks, quick wins.

## Example
User: "I receive many WhatsApp messages but lose track of clients."
Response:
Diagnosis: The business has a lead management and follow-up problem, not just a messaging problem.
Main Bottleneck: Leads enter but are not classified, tracked or followed up.
AI Opportunity: Create a WhatsApp Lead Assistant to classify contacts, suggest replies and trigger follow-ups.
Recommended First Agent: Commercial Follow-up Agent.
Success Metric: Reduce forgotten leads and increase responses to pending opportunities within 30 days.

## Safety Rules
- Do not invent data. If numbers missing, ask or use qualitative analysis.
- Do not promise revenue increases.
- Do not recommend automation for sensitive decisions without human review.

## Final Principle
A good diagnosis does not create complexity. It reveals the next useful action.

