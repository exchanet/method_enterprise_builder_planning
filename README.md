# Method Enterprise Builder Planning

> **Universal 8-phase methodology for planning and building enterprise-grade, mission-critical, and high-availability software systems. Compatible with leading AI coding agents.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Tests](https://img.shields.io/badge/tests-75%20passing-success)](.)
[![Coverage](https://img.shields.io/badge/coverage-%E2%89%A599%25-success)](.)
[![Multi-Agent](https://img.shields.io/badge/agents-5%20platforms-purple)](agents/)

**Version:** 2.0.0 | **License:** MIT | **Language:** 🇬🇧 EN / 🇪🇸 ES

**Author:** Francisco J Bernades  
**GitHub:** [@exchanet](https://github.com/exchanet)  
**Repository:** [method_enterprise_builder_planning](https://github.com/exchanet/method_enterprise_builder_planning)

---

## 🌟 Why use this method?

### For teams building:
- **Banking & Fintech**: Payment gateways, trading platforms, regulatory compliance systems
- **Healthcare**: HIPAA-compliant patient records, telemedicine platforms, medical device software
- **E-commerce at scale**: Multi-tenant SaaS, high-traffic marketplaces, distributed inventory systems
- **Government & Defense**: Security-first systems, audit trails, mission-critical infrastructure
- **Enterprise SaaS**: Multi-region deployments, 99.99% SLA requirements, GDPR/SOC2 compliance

### What you get:
- ✅ **Systematic architecture decisions** documented as ADRs with rejected alternatives
- ✅ **Risk identification** (STRIDE threat model) before writing code
- ✅ **Micro-task decomposition** (≤50 lines) for parallel development
- ✅ **Test strategy** with ≥99% coverage requirements
- ✅ **Compliance mapping** (ISO 27001, GDPR, PCI-DSS, SOC2)
- ✅ **Automated quality gates** via CI/CD templates
- ✅ **Evidence-based delivery** with metrics and sign-off reports

---

## Recommended companion methods

- [Method Modular Design](https://github.com/exchanet/method_modular_design) — Core + Packs architecture pattern
- [PDCA-T Method](https://github.com/exchanet/method_pdca-t_coding) — Quality assurance cycle (≥99% test coverage)

---

## What is this?

**Method Enterprise Builder Planning** is a **universal hybrid framework** combining:
- **Structured prompt system** for AI coding agents (Cursor AI, Claude Code, Kimi Code, Windsurf, Google Antigravity)
- **Standalone executable tools** (ADR Validator, Microtask Linter) for automated quality gates
- **CI/CD integration templates** for GitHub Actions, GitLab CI, Azure DevOps, and Jenkins

The name **Builder** reflects the method's comprehensive scope: it doesn't just *plan* — it orchestrates the complete *construction* of enterprise-grade software, from initial stakeholder analysis through architecture decisions, security hardening, micro-task decomposition, test strategy (≥99% coverage), and evidence-based delivery sign-off.

### Multi-agent architecture

Unlike agent-specific frameworks, this methodology works across **5 leading AI coding platforms**:

| Agent Platform | Adapter | Installation |
|---|---|---|
| **Cursor AI** | `.cursor/` rules + skills | Express install or manual |
| **Claude Code** | `CLAUDE.md` + `.claude/` | Copy to project root |
| **Kimi Code** | `KIMI.md` | Single file |
| **Windsurf Cascade** | `WINDSURF.md` | Single file |
| **Google Antigravity** | `AGENTS.md` + `GEMINI.md` + `.agent/skills/` | Full skills package |

All adapters follow the **same 8-phase protocol**, ensuring consistency regardless of which AI agent you use.

### Hybrid nature: Prompts + Executables

**Structured prompts** guide the agent through systematic planning phases.  
**Executable tools** provide deterministic validation that complements agent judgment:

- **ADR Validator**: 11 enterprise rules (structural, business, compliance) — blocks Accepted status if requirements not met
- **Microtask Linter**: Enforces ≤50 effective lines per file, suggests automatic splits
- **CI/CD Gates**: Automated quality checks in your pipeline

**What this guarantees:** A systematic 8-phase planning process with automated quality enforcement at critical gates.

**What it does not guarantee:** Bit-perfect identical outputs on every run. The agent applies architectural judgment within the structure — which is the intended behavior for complex system design.

### Target software quality levels

| Standard | Description |
|---|---|
| Enterprise-grade | Large-scale, high-user-load, complex transactions, strict security |
| Mission-critical | Failure has catastrophic financial or operational impact |
| High-availability | 99.999% uptime architecture (5 nines HA design) |
| Security by design | Security integrated from architecture, not bolted on after |
| Scalable system engineering | Handles massive data and transaction growth without performance loss |
| ACID Compliance | Atomicity, Consistency, Isolation, Durability for all transactions |
| RegTech / Compliance | ISO 27001, ISO/IEC 25000 (SQuaRE), CMMI level 3+, GDPR, SOC2, PCI-DSS |

---

## 🚀 v2.0.0 — From Cursor-only to universal multi-agent framework

| Component | What it does | Why it matters |
|---|---|---|
| **Multi-Agent Support** | Cursor AI, Claude Code, Kimi Code, Windsurf, Google Antigravity | Use with **any leading AI coding agent** — same methodology, same 8 phases |
| **ADR Validator** | CLI tool: 11 enterprise rules (structural, business, compliance) | **Automated architecture quality gate** — blocks Accepted status if requirements not met |
| **Microtask Linter** | Enforces ≤50 effective lines per file | **Enables parallel development** — suggests automatic splits for oversized files |
| **CI/CD Templates** | Ready-to-use: GitHub Actions, GitLab CI, Azure DevOps, Jenkins | **Quality gates in your pipeline**: coverage check, microtask linting, delivery validation |
| **Executable Tools** | TypeScript validators with ≥99% test coverage | **Deterministic validation** — not just prompts, real automation |

### Migration from v1.x

> **Breaking change:** Directory structure refactored for multi-agent support.  
> **Old:** `.cursor/` in root  
> **New:** `agents/cursor/.cursor/`, `agents/claude-code/`, `agents/antigravity/`, etc.

**Automatic migration:**
```bash
# Windows
powershell -File scripts/migrate-to-v2.ps1

# macOS / Linux
bash scripts/migrate-to-v2.sh
```

See [MIGRATION-v2.md](docs/MIGRATION-v2.md) for detailed migration guide.

---

## 📚 See it in action

### Complete executed walkthrough

Read the **[Banking Payment Authorization walkthrough](examples/banking-walkthrough.md)** — a **real agent session** building an enterprise payment system from scratch:

- **Phase 1**: Stakeholder map (product, security, compliance, DevOps)
- **Phase 2**: Micro-task backlog (32 tasks, ≤50 lines each)
- **Phase 3**: Risk analysis (STRIDE threat model: SQL injection, MITM, privilege escalation)
- **Phase 4-5**: 7 ADRs with rejected alternatives (database choice, encryption, idempotency)
- **Phase 6**: TypeScript implementation with ≥99% test coverage
- **Phase 7**: Delivery report with metrics and compliance evidence
- **Phase 8**: Handover documentation for production deployment

**No placeholders, no synthetic examples.** Real outputs generated by the methodology.

---

## 🏗️ What you can build with this

### Examples by industry

| Domain | System Example | Key Requirements Addressed |
|---|---|---|
| **Banking** | Payment authorization gateway | PCI-DSS compliance, ACID transactions, fraud detection, audit trails |
| **Healthcare** | Electronic health records (EHR) | HIPAA compliance, data encryption, role-based access, consent management |
| **E-commerce** | Multi-tenant marketplace | Horizontal scaling, eventual consistency, idempotency, rate limiting |
| **Insurance** | Claims processing workflow | State machine design, SLA tracking, regulatory reporting, disaster recovery |
| **Supply Chain** | Real-time inventory tracking | High-availability architecture, distributed transactions, conflict resolution |
| **Government** | Citizen identity verification | Security by design, zero-trust architecture, GDPR compliance, penetration testing |

### Technical patterns covered

- **Architecture**: Microservices, event-driven, CQRS, saga patterns, API gateway
- **Data**: ACID transactions, eventual consistency, sharding, replication, data lakes
- **Security**: Zero-trust, encryption at rest/in-transit, RBAC, OAuth2/OIDC, audit logs
- **Scalability**: Horizontal scaling, caching strategies, CDN, load balancing
- **Compliance**: GDPR, HIPAA, PCI-DSS, SOC2, ISO 27001 mapping

---

## Quick Start

### Express installation (recommended)

**For Cursor AI**:
1. Download repository as `.zip` from [GitHub](https://github.com/exchanet/method_enterprise_builder_planning) → unzip
2. Copy folder path (e.g., `C:\Users\your-name\Downloads\method-enterprise_builder_planning`)
3. Cursor → New Agent chat → Paste path:
   ```
   Install this method globally: C:\Users\your-name\Downloads\method-enterprise_builder_planning
   ```
4. Restart Cursor → Use with: `/method-enterprise_builder`

**For other agents**:

```bash
# Clone repository
git clone https://github.com/exchanet/method_enterprise_builder_planning.git
cd method_enterprise_builder_planning

# Install for your agent
bash scripts/migrate-to-v2.sh --project=/path/to/your-project --agent=cursor
# Options: cursor, claude-code, kimi-code, windsurf, antigravity
```

**Global installation** (available in all projects):
```bash
# Cursor AI
cp -r agents/cursor/.cursor ~/.cursor/

# Claude Code
cp agents/claude-code/CLAUDE.md ~/.config/claude/
cp -r agents/claude-code/.claude ~/.config/claude/

# Antigravity
cp agents/antigravity/AGENTS.md ~/.config/antigravity/
cp -r agents/antigravity/.agent ~/.config/antigravity/
```

See [agents/README.md](agents/README.md) for detailed installation per platform.

### Manual installation

```bash
# Clone repository
git clone https://github.com/exchanet/method_enterprise_builder_planning.git
cd method_enterprise_builder_planning

# Copy agent-specific files to your project
# For Cursor AI:
cp -r agents/cursor/.cursor /path/to/your/project/

# For Claude Code:
cp agents/claude-code/CLAUDE.md /path/to/your/project/
cp -r agents/claude-code/.claude /path/to/your/project/

# For Antigravity:
cp agents/antigravity/AGENTS.md /path/to/your/project/
cp agents/antigravity/GEMINI.md /path/to/your/project/
cp -r agents/antigravity/.agent /path/to/your/project/
```

Also install the companion methods:

```bash
# Method Modular Design (Core + Packs pattern)
git clone https://github.com/exchanet/method_modular_design.git
cp -r method_modular_design/agents/cursor/.cursor /path/to/your/project/

# PDCA-T Method (quality assurance cycle)
git clone https://github.com/exchanet/method_pdca-t_coding.git
cp -r method_pdca-t_coding/agents/cursor/.cursor/rules/METODO-PDCA-T.md /path/to/your/project/.cursor/rules/
cp -r method_pdca-t_coding/agents/cursor/.cursor/skills/metodo-pdca-t /path/to/your/project/.cursor/skills/
```

---

## Activation

Once installed, activate with any of these phrases:

```
/method-enterprise_builder

"Plan enterprise feature: [description]"
"Design mission-critical [system type]"
"Create ACID-compliant module for [feature]"
"Build high-availability [component] with 99.99% SLA"
"Implement security-first [module] with audit trail and GDPR compliance"
```

Cursor will guide you through the complete 8-phase cycle automatically.

---

## The 8-Phase Builder Cycle

```
PHASE 1: Enterprise Context Analysis
         │  System classification · Stakeholders · Regulatory environment
         ▼
PHASE 2: Non-Functional Requirements (NFR)
         │  Performance SLOs · Availability SLA · Scalability · Security · Compliance
         ▼
PHASE 3: Risk Matrix
         │  STRIDE threat model · Technical risk catalog · Mitigations
         ▼
PHASE 4: Micro-Task Decomposition (PDCA-T)
         │  Feature → Domain → Layer → ≤50-line micro-tasks with dependency DAG
         ▼
PHASE 5: Architecture Decisions (ADR)
         │  Pattern selection · C4 diagrams · Pack mapping · ADR per decision
         ▼
PHASE 6: Security & Compliance Mapping
         │  STRIDE per module · RBAC matrix · ACID boundaries · Compliance matrix
         ▼
PHASE 7: Test Strategy
         │  Test pyramid · Coverage gates · Load tests · CI quality gates
         ▼
PHASE 8: Delivery Report
         │  Evidence-based sign-off · Test metrics · Security · Compliance checklist
```

---

## Repository Structure

```
method-enterprise_builder_planning/
├── .cursor/
│   ├── rules/
│   │   ├── METHOD-ENTERPRISE-BUILDER-PLANNING.md  ← main rule (trigger: manual)
│   │   ├── ENTERPRISE_ARCHITECTURE.md
│   │   ├── ENTERPRISE_SECURITY.md
│   │   ├── ENTERPRISE_SCALABILITY.md
│   │   ├── ENTERPRISE_COMPLIANCE.md
│   │   ├── ENTERPRISE_TESTING.md
│   │   └── ENTERPRISE_MICROTASK_PLANNER.md
│   └── skills/
│       └── method-enterprise-builder-planning/
│           ├── SKILL.md                        ← main orchestrator skill
│           ├── architecture-planning.md
│           ├── security-planning.md
│           ├── scalability-planning.md
│           ├── compliance-planning.md
│           ├── microtask-decomposition.md
│           ├── testing-strategy.md
│           └── delivery-report.md
├── core/
│   └── planning-engine/                        ← core layer (infrastructure only)
├── packs/
│   ├── enterprise-architecture-pack/
│   ├── security-compliance-pack/
│   ├── high-availability-pack/
│   ├── testing-coverage-pack/
│   └── acid-compliance-pack/
├── examples/
│   ├── banking-walkthrough.md        ← ✅ complete executed walkthrough (start here)
│   ├── banking-system-plan.md
│   ├── high-availability-saas-plan.md
│   └── mission-critical-api-plan.md
├── docs/
│   ├── INSTALLATION.md
│   ├── USAGE.md
│   └── ENTERPRISE-STANDARDS-REFERENCE.md
├── README.md
└── README.es.md
```

---

## Executable tools (v2.0.0)

### ADR Validator

Validates Architecture Decision Records against 11 enterprise rules before marking them Accepted.

```bash
# Validate all ADRs in your project
node packs/enterprise-architecture-pack/validators/adr-validator/src/index.ts docs/adr/

# CI/CD (JUnit XML output)
node packs/enterprise-architecture-pack/validators/adr-validator/src/index.ts \
  --format=junit --output=reports/adr-results.xml docs/adr/
```

### Microtask Linter

Validates that source files comply with the ≤50 effective lines rule, with split suggestions.

```bash
# Validate a single file
node packs/enterprise-microtask-planner-pack/validators/microtask-linter/src/index.ts \
  --task=src/payments/domain/money.ts

# Validate all files in a directory
node packs/enterprise-microtask-planner-pack/validators/microtask-linter/src/index.ts \
  --dir=src/ --recursive
```

### CI/CD Quality Gates

```bash
# Copy GitHub Actions workflow to your project
cp .ci-cd/templates/github-actions/workflow-enterprise-builder.yml \
   .github/workflows/enterprise-builder.yml
```

Available for: GitHub Actions, GitLab CI, Azure DevOps, Jenkins. See [.ci-cd/README.md](.ci-cd/README.md).

---

## Configuration schemas and `x-ui` properties

Each pack and the Core include a `config.schema.json` that documents configurable parameters.
Some fields carry `x-ui` annotations (e.g. `"widget": "slider"`, `"widget": "checkbox-group"`).

**These are design markers for a future configuration UI — no GUI currently renders them.**
They serve two purposes today: documenting the intended UX for each field, and helping the
Cursor AI agent describe options in natural language. They have no runtime effect.

---

## Available Packs

| Pack | Activated in phase | Provides |
|---|---|---|
| `enterprise-architecture-pack` | Phase 5 | ADR templates, C4 diagrams, pattern decision trees |
| `security-compliance-pack` | Phase 3, 6 | STRIDE templates, RBAC matrices, audit checklists |
| `high-availability-pack` | Phase 2, 5 | SLA/SLO definitions, failover strategies, chaos engineering |
| `testing-coverage-pack` | Phase 4, 7 | Test pyramid, coverage requirements, load test templates |
| `acid-compliance-pack` | Phase 4, 6 | Transaction boundaries, rollback strategies, idempotency |

---

## Related Methods

| Method | Role |
|---|---|
| [Method Modular Design](https://github.com/exchanet/method_modular_design_cursor) | Architecture pattern (Core + Packs) used for all generated code |
| [PDCA-T Method](https://github.com/exchanet/method_pdca-t_coding_Cursor) | Quality cycle (≥99% coverage) applied to every micro-task |

---

## License

MIT — see [LICENSE](LICENSE) file.

---

## Author

**Francisco J Bernades**  
GitHub: [@exchanet](https://github.com/exchanet)
