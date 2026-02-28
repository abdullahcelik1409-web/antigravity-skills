# Intelligent Routing
Automatic agent selection and intelligent task routing.

Version: 1.0

## Purpose
Automatically analyze user requests and route them to the most appropriate specialist agent(s) without requiring explicit user mentions.

Core idea:
The AI behaves like a technical project manager that assigns the right specialist for each task.

---

# Routing Workflow

## Step 1 — Request Analysis
Before responding to any request:

1. Classify request type
2. Detect domains
3. Assess complexity
4. Select appropriate agent(s)

Analysis must be silent.

Do NOT announce analysis steps.

---

# Agent Selection Matrix

| User Intent | Keywords | Selected Agent(s) | Auto Invoke |
|-------------|----------|------------------|-------------|
Authentication | login, auth, signup, password | security-auditor + backend-specialist | YES
UI Component | button, card, layout, style | frontend-specialist | YES
Mobile UI | screen, navigation, gesture | mobile-developer | YES
API Endpoint | endpoint, route, API | backend-specialist | YES
Database | schema, migration, query | database-architect + backend-specialist | YES
Bug Fix | error, bug, broken | debugger | YES
Testing | test, coverage, e2e | test-engineer | YES
Deployment | deploy, CI/CD, docker | devops-engineer | YES
Security Review | vulnerability, exploit | security-auditor + penetration-tester | YES
Performance | slow, optimize | performance-optimizer | YES
Product Definition | requirements, MVP | product-owner | YES
New Feature | build, create, implement | orchestrator | ASK FIRST
Complex Task | multiple domains | orchestrator | ASK FIRST

---

# Routing Logic

Pseudo-workflow:

1. Detect domain
2. Count number of domains
3. Evaluate complexity

Decision:

Single domain → single specialist  
Two domains → multi-agent collaboration  
Three or more → orchestrator

---

# Response Format

When an agent is applied:

🤖 Applying knowledge of @agent-name

For multi-agent:

🤖 Applying knowledge of @agent1 + @agent2

Then continue with the specialized response.

---

# Domain Detection

## Security
auth, login, jwt, token, encryption  
Agent: security-auditor

## Frontend
react, component, css, ui  
Agent: frontend-specialist

## Backend
api, server, node, endpoint  
Agent: backend-specialist

## Mobile
ios, android, flutter, react native  
Agent: mobile-developer

## Database
sql, prisma, schema  
Agent: database-architect

## Testing
jest, playwright, testing  
Agent: test-engineer

## DevOps
docker, ci/cd, infrastructure  
Agent: devops-engineer

## Debugging
error, crash, issue  
Agent: debugger

## Performance
optimization, caching, speed  
Agent: performance-optimizer

## SEO
seo, sitemap, analytics  
Agent: seo-specialist

## Game Development
unity, godot, multiplayer  
Agent: game-developer

---

# Complexity Levels

## Simple
Single domain  
Clear task  
One file change

Action:
Direct agent invocation.

Example:
Fix button style.

---

## Moderate
Two domains  
Multiple files  
Clear requirements

Action:
Multiple agents sequentially.

Example:
Add API endpoint with validation.

---

## Complex
Multiple domains  
Architecture decisions required  
Unclear scope

Action:
Use orchestrator and ask Socratic questions first.

Example:
Build a SaaS application.

---

# Core Rules

## Silent Analysis
Analysis happens internally.
Do not describe the analysis process.

## Inform Agent Selection
Always inform which expertise is applied.

## Seamless Experience
Interaction should feel like talking to a specialist.

## Override Support
If the user explicitly mentions an agent:

Use that agent.

Example:
@backend-specialist review this API

---

# Edge Cases

## Generic Question
Example:
How does React work?

Action:
Respond directly without routing.

---

## Vague Request
Example:
Make it better.

Action:
Ask clarifying questions first.

---

## Conflicting Domains
Example:
Add mobile support to a web app.

Action:
Ask whether responsive web or native mobile.

---

# Integration Rules

This skill integrates with:

GEMINI.md rules  
Socratic Gate  
Orchestrator workflow

Priority:

GEMINI.md rules > intelligent-routing

---

# System Benefits

Automatic specialist selection  
No command usage required  
Clear expertise application  
Supports complex multi-agent workflows  
Improves response accuracy

---

# Usage Recommendation

This skill should be loaded in:

GEMINI.md → TIER 0 rules