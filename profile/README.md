# projectious.work

**Turning emerging technical capabilities into predictable, auditable delivery.**

Projectious is an independent initiative exploring how AI changes the economics,
organisation, and governance of technical work — and what infrastructure,
operating models, and delivery mechanisms are needed to make those changes
reliable.

The work deliberately combines organisational questions with technical
experiments. Some repositories are usable tools, some are applied research, and
some are explicitly labelled prototypes or early-development work. Status,
validation, and limitations are part of the evidence.

## Start here

| Project | Role in the initiative | Current status |
|---|---|---|
| [aibox](https://github.com/projectious-work/aibox) | Reproducible, terminal-first AI development workspaces from a declarative project contract | Usable project — maintained v0.x; v1 direction under active development |
| [processkit](https://github.com/projectious-work/processkit) | Provider-neutral process memory, skills, schemas, and MCP tools for agentic software projects | Stable lifecycle — actively maintained, pre-1.0 |
| [ainfra](https://github.com/projectious-work/ainfra) | Inspectable infrastructure provisioning with reviewed plans and explicit lifecycle controls | Early development — exercised on disposable Hetzner infrastructure |
| [ai-market-research](https://github.com/projectious-work/ai-market-research) | Inspectable decision support for AI models, harnesses, configurations, and self-hosting choices | Applied research — actively maintained |
| [kubeclaw](https://github.com/projectious-work/kubeclaw) | Learning prototype for isolation, network policy, and safe infrastructure boundaries for agent workloads | Prototype — not production ready |

Supporting work includes the [Projectious brand system](https://github.com/projectious-work/brand),
the emerging [Projectious Hugo theme](https://github.com/projectious-work/brand-theme-hugo-vanilla),
and additional experiments such as [kaits](https://github.com/projectious-work/kaits).

## Where this is going

The current technical direction separates responsibilities deliberately rather
than building one large platform:

```text
infrastructure target
        │
        ▼
      ainfra
provision + configure
        │
        ▼
       aibox
build + deploy reproducible AI workspaces
        │
        ▼
    processkit
process memory + skills + validated agent workflows
        │
        ▼
AI harnesses / agents
        │
        ▼
projects, research, and organisation-specific tools
```

This is a direction of travel, not a claim that the whole stack is already a
single integrated production platform.

- **ainfra** owns infrastructure provisioning and target contracts; it does not
  own workload images or agent process semantics.
- **aibox** owns reproducible workspace images, tooling, runtime configuration,
  and the direction toward backend-neutral deployment; it does not provision
  cloud infrastructure.
- **processkit** owns process semantics: project memory, skills, schemas,
  validated state transitions, and MCP surfaces; it does not own model-provider
  APIs or workspace infrastructure.
- AI harnesses remain replaceable integration targets rather than architectural
  owners of project context.

## What Projectious is exploring

The repositories support a broader set of working theses rather than a generic
"AI tools" portfolio. Current questions include:

- **The minimum viable enterprise is changing.** One person working with
  multiple specialised agents may be able to coordinate increasingly
  sophisticated work.
- **The economics of software quality are changing.** If iteration becomes
  cheaper, the economically reasonable tolerance for poor software should fall.
- **The build-versus-buy boundary may move.** Agent-assisted engineering can
  make narrower, organisation-specific software viable in more cases.
- **Operating models become more programmable.** Processes, policies, memory,
  controls, and decision mechanisms increasingly gain machine-readable
  representations that agents can act upon.
- **Governance increasingly moves into the system.** Provenance, validation,
  permissions, process memory, and decision evidence can become executable and
  observable parts of delivery rather than only documents and meetings.

These are theses to test and refine, not settled predictions.

## How the work is developed

Projectious is led by **Bernhard Gerlach**, an Operations, Transformation, and
Technical Program leader extending operating-model experience into AI-assisted
delivery, agent infrastructure, and reproducible technical workflows.

AI tools assist research, implementation, testing, and documentation. Problem
framing, architecture boundaries, portfolio decisions, evidence standards, and
final accountability remain human responsibilities.

A useful shorthand for the territory is:

**Agentic AI. Agile. Cloud.**

Not as three service lines: agentic AI changes the unit and economics of
productive work; Agile contributes iterative learning and short feedback loops;
Cloud provides programmable infrastructure. Operating models, governance, and
accountability connect them into reliable delivery.

## Evidence before claims

The presence of a repository does **not** imply customer adoption, production
operation, security assurance, enterprise support, or commercial product
maturity.

For each project, follow its own README, status page, validation evidence,
releases, tests, and limitations. Prototype and early-development labels are
intentional.
