# fullstack-agents
**Work in progress**: Agentic Orchestration to automate end-to-end fullstack workflow: from gathering requirement to deployment and maintainance.
## Structure
``` 
main-project/
├── .agents/
│   ├── orchestrator/
│   │   └── NICK_FURY.md
│   ├── roles/
│   │   ├── SHIELD_REQUIREMENTS.md
│   │   ├── CAPTAIN_AMERICA_COMPLIANCE.md
│   │   ├── TONY_STARK_DEVELOPER.md
│   │   └── HULK_TESTER.md
│   ├── skills/
│   │   ├── GRILL_ME.md           <-- by mattpocock/grill-me
│   │   ├── PONYTAIL.md           <-- by DietrichGebert/ponytail
│   │   └── CAVEMAN.md            <-- by JuliusBrussee/caveman
│   ├── state/
│   │   ├── pipeline_status.md
│   │   ├── requirements_spec.md
│   │   ├── compliance_policy.md
│   │   ├── work_orders.md
│   │   └── test_report.md
│   └── README.md
├── src/                          <-- Tony writes application code here
└── tests/                        <-- Hulk outputs test cases here
```
## Workflow
```
Client Brief (Raw Idea)
       │
       ▼
[01_SHIELD.md] ──(grill-me)──► S.H.I.E.L.D. (Requirement Gathering)
                                      │
                                      ▼
                             requirements_spec.md
                                      │
                                      ▼
[00_NICK_FURY.md] ──────────► Nick Fury (Plan & Task Breakdown)
                                      │
                                      ▼
                                work_orders.md
                                      │
       ┌──────────────────────────────┴──────────────────────────────┐
       ▼                                                             ▼
[02_CAPTAIN_AMERICA.md]                                     [03_TONY_STARK.md]
Compliance & Guardrails                                     Senior Fullstack Dev
(Data privacy, secrets, rules)                             (Ponytail + Caveman)
       │                                                             │
       └──────────────────────────────┬──────────────────────────────┘
                                      ▼
                              Working Codebase
                                      │
                                      ▼
[04_HULK.md] ───────────────► Hulk (Brute Force QA & Edge Cases)
                                      │
                                      ▼
                               test_report.md
                                      │
                                      ▼
                           Nick Fury (Final Sign-off)
```
## n8n Workflow
<img width="1039" height="377" alt="image" src="https://github.com/user-attachments/assets/74e9c847-f20d-4dbb-85e0-03fff2ed81db" />

## Note
- More agents (avengers) will be added soon (e.g. for documentation, deployment, monitoring, etc)
- Open to suggestions/discussion 
