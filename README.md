# ai-incident-triage-assistant

A learning prototype: a local, AI-assisted incident triage tool. A simulated alert goes in, and the tool suggests a severity, an investigation checklist and a runbook to follow.

**This is a learning prototype. It does not autonomously perform production remediation.**

## Status
Just started. Nothing is built yet.

## Planned design
- A FastAPI endpoint that receives a simulated alert
- A small knowledge base of 3 to 5 incident runbooks, searched with retrieval (RAG)
- Safe mock tools only, with no real systems behind them
- A human must approve before any action is taken

## Safety rules
- No real cloud credentials and no shell access
- Every tool is a mock that returns sample data
- Documenting prompt injection, secrets handling, least privilege, cost limits and logging

## Rules I follow
- I write the code myself and test everything.
- No secrets are committed.
