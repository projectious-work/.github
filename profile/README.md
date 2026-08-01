# Projectious

Projectious explores and builds the technical and organizational layers
required to turn emerging AI capabilities into reproducible, governed, and
auditable ways of working.

The work connects operating-model design—responsibilities, controls,
repeatability, sourcing, and auditability—with concrete technical mechanisms.
Some repositories are usable tools, others are applied research or explicitly
labelled prototypes. Their status and limitations are part of the evidence.

## Start here

| Project | What it demonstrates | Status |
|---|---|---|
| [aibox](https://github.com/projectious-work/aibox) | Reproducible, terminal-first AI development workspaces generated from a declarative project contract | Usable project — active development |
| [processkit](https://github.com/projectious-work/processkit) | Provider-neutral process memory, validated project state, skills, and MCP tools for coding agents | Usable project — active development, pre-1.0 |
| [ai-market-research](https://github.com/projectious-work/ai-market-research) | Sourced, inspectable decision support for models, harnesses, subscriptions, and self-hosting choices | Applied research — actively maintained |
| [kubeclaw](https://github.com/projectious-work/kubeclaw) | A learning prototype exploring infrastructure isolation and network policy for agent workloads | Working prototype — not production ready |

Additional experiments and supporting assets include
[kaits](https://github.com/projectious-work/kaits),
[ainfra](https://github.com/projectious-work/ainfra),
the [Projectious Brand project](https://github.com/projectious-work/brand), and
the [public website](https://github.com/projectious-work/website). Experimental
repositories should be read according to the status and limitations stated in
their own README.

## How the layers relate

```text
secure infrastructure targets
        │
        ▼
reproducible workspace images and deployments       aibox
        │
        ▼
governed project memory and agent workflows         processkit
        │
        ▼
evidence-based technical and sourcing decisions     applied research
```

The projects are deliberately separated by responsibility. Infrastructure
templates provision targets; aibox builds and deploys workspaces; processkit
owns process content and its installation; research repositories make
decision evidence inspectable.

## About the work

Projectious is led by Bernhard Gerlach, an Operations, Transformation, and
Technical Program leader extending operating-model expertise into AI-assisted
delivery, agent infrastructure, and reproducible technical workflows.

AI tools assist parts of the research, implementation, and documentation.
Problem framing, architecture boundaries, portfolio decisions, review, and
the standard of evidence remain human responsibilities. Each repository should
document its own validation and limitations rather than relying on this profile
for maturity claims.

## What this portfolio does not claim

The presence of a repository does not imply customer adoption, production
operation, security assurance, or enterprise support. Prototype and research
labels are intentional. Follow each project’s quick start, tests, releases,
and limitations for the current evidence.

Learn more at [projectious.work](https://projectious.work).
