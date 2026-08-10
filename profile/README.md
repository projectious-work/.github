# projectious.work

**Turning emerging technical capabilities into predictable, auditable delivery.**

projectious.work is an independent initiative exploring how AI changes the economics,
organisation, and governance of technical work — and what infrastructure,
operating models, memory systems, orchestration, and delivery mechanisms are needed
to make those changes reliable.

The work deliberately combines organisational questions with technical
experiments. Some repositories are usable tools, some are applied research, and
some are explicitly labelled prototypes or early-development work. Status,
validation, and limitations are part of the evidence.

## Start here

| Project | Role in the initiative | Current status |
|---|---|---|
| [aibox](https://github.com/projectious-work/aibox) | Reproducible, terminal-first AI development workspaces from a declarative project contract | Usable project — maintained v0.x; v1 direction under active development |
| [processkit](https://github.com/projectious-work/processkit) | Provider-neutral process memory, skills, schemas, and MCP tools for agentic software projects | Maintained v0.x; v1 direction under active development |
| [ainfra](https://github.com/projectious-work/ainfra) | Security-oriented remote infrastructure for agent workloads: controlled execution environments with explicit inbound/outbound network policy, reviewed provisioning, and reproducible teardown | Early development — exercised on disposable Hetzner infrastructure |
| [ai-market-research](https://github.com/projectious-work/ai-market-research) | Inspectable decision support for AI models, harnesses, configurations, and self-hosting choices | Applied research — actively maintained |
| [kubeclaw](https://github.com/projectious-work/kubeclaw) | Learning prototype for isolation, network policy, and safe infrastructure boundaries for agent workloads | Prototype — not production ready |

Supporting work includes the [projectious.work brand system](https://github.com/projectious-work/brand)
(**complete brand and design system with tokens, assets, templates, and published documentation — active/released, v1.0**),
[kaits](https://github.com/projectious-work/kaits)
(**RPG-inspired multi-agent organisation and orchestration experiment with roles, departments, task routing, budgets, autonomy, lifecycle hooks, and an event-driven UI — substantial working prototype; not a production platform**),
and **airunner**
(**concept for a lightweight agent runtime/execution layer — idea/private stub; no public implementation yet**).

## Where this is going

The current technical direction separates responsibilities deliberately rather
than building one large platform. The first layers already exist in different
stages of maturity; the upper layers describe the scaling direction and should
be read as architecture hypotheses rather than implemented products.

```text
infrastructure targets
        │
        ▼
      ainfra
secure remote execution environment + network controls
        │
        ▼
       aibox
build + deploy reproducible AI workspaces
        │
        ▼
    processkit
project/process memory + skills + validated workflows
        │
        ▼
   memory layers
working memory · project memory · organisational memory
        │
        ▼
AI harnesses / specialised agents
        │
        ▼
 orchestration layer
agent selection · delegation · supervision · hand-off · recovery
        │
        ▼
projects, research, and organisation-specific software
```

This is a direction of travel, not a claim that the whole stack is already a
single integrated production platform.

### Current foundations

- **ainfra** explores a security-oriented alternative to running capable agents
  directly on local machines. It provisions controlled remote execution targets
  with explicit lifecycle boundaries and deliberate inbound/outbound network
  configuration, so agent workloads can be isolated from the user's everyday
  workstation and exposed only through reviewed access paths. Its current scope
  remains infrastructure provisioning and target contracts; it does not own
  workload images or agent process semantics.
- **aibox** owns reproducible workspace images, tooling, runtime configuration,
  and the direction toward backend-neutral deployment; it does not provision
  cloud infrastructure.
- **processkit** owns project/process semantics: structured memory, skills,
  schemas, validated state transitions, and MCP surfaces; it does not own
  model-provider APIs or workspace infrastructure.
- AI harnesses remain replaceable integration targets rather than architectural
  owners of project context.

### Scaling questions under exploration

The next scaling problem is not simply “more agents”. It is how to preserve
context, accountability, and useful autonomy as more specialised agents work
across longer-lived tasks and larger organisations.

Areas under exploration include:

- **Multi-layer memory.** Distinguish ephemeral working context from durable
  project memory and broader organisational memory. Different layers need
  different retention, validation, access, provenance, and summarisation rules.
- **Orchestration above the agent layer.** Coordinate specialised agents without
  turning one central prompt or one monolithic supervisor into the new
  bottleneck. The orchestration layer selects and combines available harnesses
  and agents, delegates work, supervises execution, manages hand-offs, retries,
  escalation, recovery, and human intervention.
- **Shared organisational context.** Give multiple agents a reliable way to work
  from the same decisions, policies, constraints, interfaces, and history while
  avoiding silent divergence between local context copies.
- **Executable governance.** Move more controls, permissions, validation,
  provenance, and decision evidence into the technical system so that scaling
  does not depend on adding equivalent layers of meetings and manual review.
- **Human accountability with agent autonomy.** Increase what agents may do
  independently while keeping decision ownership, exceptions, and escalation
  visible to humans.
- **Composable agent teams.** Treat agents and tools as replaceable capabilities
  that can be assembled around a task, rather than as one permanently fixed
  assistant or vendor-specific stack.

These ideas may become additional repositories or may remain cross-cutting
capabilities across aibox, processkit, ainfra, and future projectious.work
projects. Repository boundaries should follow responsibility, not marketing.

## projectious.work's core theses

The technical stack exists to test a broader set of theses about future
organisations and software, not to create a generic “AI tools” portfolio.

Current working theses include:

- **The minimum viable enterprise is changing.** One person working with
  multiple specialised agents may be able to coordinate increasingly
  sophisticated work, making very small AI-native organisations viable for more
  classes of products and services.
- **AI changes what is economically viable, not only what can be automated.**
  The larger effect may be a shift in viable organisational forms, software
  strategies, quality expectations, and delivery mechanisms.
- **The economics of software quality are changing.** If iteration, testing,
  documentation, and refinement become materially cheaper, the economically
  reasonable tolerance for poor software should fall with them.
- **The build-versus-buy boundary may move.** Agent-assisted engineering can
  make narrower, organisation-specific software viable in more cases where
  configured standard software previously won primarily on cost.
- **“Software of One” becomes a meaningful design space.** Software tailored to
  one organisation, team, workflow, or even individual may become economically
  maintainable when agents carry a substantial share of implementation and
  maintenance work.
- **Operating models become more programmable.** Processes, policies, roles,
  memory, controls, and decision mechanisms increasingly gain machine-readable
  representations that agents can act upon.
- **Governance increasingly moves into the system.** Provenance, validation,
  permissions, process memory, and decision evidence can become executable and
  observable parts of delivery rather than only documents and meetings.
- **AI adoption is an operating-model problem.** Models and tools become durable
  organisational capability only when responsibilities, decision rights,
  governance, context, evaluation, security, feedback loops, and accountability
  evolve with them.

These are theses to test, challenge, and refine — not settled predictions.

## How the work is developed

projectious.work is led by **Bernhard Gerlach**, an Operations, Transformation,
and Technical Program leader extending operating-model experience into
AI-assisted delivery, agent infrastructure, reproducible technical workflows,
and AI-enabled organisational design.

AI tools assist research, implementation, testing, and documentation. Problem
framing, architecture boundaries, portfolio decisions, evidence standards, and
final accountability remain human responsibilities.

A useful shorthand for the territory is:

**Agentic AI. Agile. Cloud.**

Not as three service lines: agentic AI changes the unit and economics of
productive work; Agile contributes iterative learning and short feedback loops;
Cloud provides programmable infrastructure. Operating models, memory,
orchestration, governance, and accountability connect them into reliable
delivery.

## Evidence before claims

The presence of a repository does **not** imply customer adoption, production
operation, security assurance, enterprise support, or commercial product
maturity.

For each project, follow its own README, status page, validation evidence,
releases, tests, and limitations. Prototype and early-development labels are
intentional.
