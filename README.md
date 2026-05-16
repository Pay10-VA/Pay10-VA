# Hey there 👋
I'm Payton — a Software Engineer with experience building customer-facing 
production applications with millions of daily requests. I specialize in 
backend development, distributed systems, and real-time data pipelines.

[![My Skills](https://skillicons.dev/icons?i=java,spring,js,ts,nodejs,express,aws,react,nextjs,mongodb,postgres,redis,kafka,docker,tailwind,html,css,github,python)](https://skillicons.dev)

<br/>

![](https://img.shields.io/badge/Role-Software_Engineer-blue)
![](https://img.shields.io/badge/Learning-AWS_SAA-FF9900?logo=amazonaws&logoColor=white)
![](https://img.shields.io/badge/Coding-Zero_Trust_API_Gateway-6366f1)

## 🛠 Recent Projects

### CoDoc | Real-Time Collaborative Document Editor
*October – November 2025 · TypeScript · Node.js · Express · Next.js · Tailwind CSS · PostgreSQL*

Full-stack collaborative document editor with conflict-free simultaneous editing 
via CRDT-based synchronization (Y.js + TipTap). Built real-time features including 
live collaborator presence, comments, and file management using Socket.IO.

---

### EventStream | Real-Time Event Analytics Platform
*March – April 2026 · Java · Spring Boot · Kafka · Redis · MongoDB · Docker · Model Context Protocol (MCP) · Python*

Real-time event ingestion and analytics platform that captures user behavior events, 
streams them through Kafka with retry and DLQ support, and persists them to MongoDB. 
Tracks live analytics using a Redis sliding window algorithm.

Also built an MCP server (FastMCP) that exposes EventStream's analytics API as 
Claude-callable tools — enabling natural language querying of funnel drop-off rates, 
top products, per-user event counts, and real-time activity.

---

### Production Readiness Skill — Claude (Internal Tool)
*May 2026 · Claude · Prompt Engineering · MCP · Process Automation*

Created a Claude Skill that automates production readiness reviews for first-release applications by performing a static source code analysis to surface missing patterns and querying the Confluence MCP server to verify required documentation to generate a pass/fail checklist with per-item findings.  It also uses the Atlassian MCP server to automatically create Jira stories to address said gaps.

---

### Foreman | Distributed Job Scheduler
*April – May 2026 · Java · Spring Boot · Kafka · PostgreSQL · Docker · Prometheus · Grafana*

Distributed job scheduler that accepts immediate, scheduled, and cron jobs via REST API and executes them by firing webhooks at the configured time. Built across three decoupled services: submission, scheduling, and execution.

Key engineering decisions: concurrent job claiming via `FOR UPDATE SKIP LOCKED`, per-job transaction isolation using `REQUIRES_NEW` propagation, at-least-once Kafka delivery with idempotency checks to minimize duplicate execution, and retry with exponential backoff and dead-letter routing. Full observability across all three services with Prometheus metrics and Grafana dashboards.

---

### Zero Pass | Zero Trust API Gateway
*May 2026 - Present (In Progress) · Java · Spring Boot · Python · gRPC · Kafka · Redis · PostgreSQL · Docker · Kubernetes · Terraform · Prometheus · Grafana · Next.js · TypeScript*

Currently in progress.
