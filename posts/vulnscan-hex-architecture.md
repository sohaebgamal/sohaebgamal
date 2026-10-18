# VulnScan-HEX: a scanner that proves, not guesses

*Sohaib Gamal · Security QA Engineer & Penetration Tester*

Most scanners tell you "this might be vulnerable." I wanted one that proves it.

So I designed and built **VulnScan-HEX** from scratch, end to end: the architecture, all 15 scanners, the CLI, the reporting and the local AI integration. It's a web vulnerability scanner in Python, built differently from many scanners.

## The difference

In many scanners, payloads, HTTP calls, parsing and verdicts live in the same code, so "found a vulnerability" can mean "the response looked interesting."

In VulnScan-HEX, the **core does one job**: it looks at real evidence and decides whether a vulnerability exists. It knows nothing about HTTP, databases or AI. Everything else plugs in through **Hexagonal Architecture (Ports & Adapters)**.

## Port vs adapter

- A **port** is a contract. It says *what* the core needs ("save a result", "generate a report") without saying how.
- An **adapter** is the implementation. It is *how* that need is met: SQLite for storage, a subprocess for running scans, a local model for AI reports.

The core only talks to ports, so any adapter can be replaced without touching the logic that decides what is vulnerable.

## What it covers

15 scanners aligned with OWASP Top 10:2025 (SQLi, XSS, SSRF, SSTI, RCE, IDOR, CSRF, JWT, GraphQL and more), 5 ports, 5 adapters, and TXT/JSON reports.

## A private AI, by design

Pentest reports contain vulnerabilities and sensitive target details, so they should never leave your machine. The AI report adapter runs a local model (DeepSeek R1 via Ollama) and talks only to localhost. No report data is sent to any external service. And because AI is just an adapter, the scanner works without it.

## Why it matters

1. **Evidence over guesses:** verdict logic lives in one place, so findings are judged consistently.
2. **Swappable parts:** new storage, report format or AI model means a new adapter.
3. **Easy to extend:** a new vulnerability class is one more scanner behind the same port.
4. **Confidential:** report data stays on your machine.

Building it myself taught me something I use in every pentest: a report full of unverified "criticals" wastes everyone's time. Verified findings get fixed.

*Built for authorized security testing only.*
