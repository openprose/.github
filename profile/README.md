![OpenProse.](https://raw.githubusercontent.com/openprose/.github/main/profile/header.png)

## Standing AI jobs, declared in Markdown.

Agent sessions end. The work they were responsible for shouldn't. **OpenProse** is a declarative language for standing AI work: you write Markdown contracts (`*.prose.md`) that declare what should stay true, and the system works out how much model work it takes to keep it that way.

It's the oldest good idea in software, pointed at agents. Like SQL, Terraform, Kubernetes, and React: you declare the desired state, and a reconciler makes reality match.

The language is harness-agnostic. Install the skill and any Prose-Complete coding agent (Claude Code, Codex CLI, OpenCode, and friends) can author and run contracts:

```bash
npx skills add openprose/prose
```

## Reactor

**Reactor** (`@openprose/reactor`) is the deterministic runtime we recommend for OpenProse. It compiles your contracts into a reactive DAG once, then re-renders only the nodes whose inputs actually moved, leaving a content-addressed receipt behind every decision. Inference cost scales with surprise, not the clock.

See it run, keyless, at zero model spend:

```bash
npx -p @openprose/reactor-devtools reactor-devtools --example surprise-cost --describe
```

## Start here

- [openprose/prose](https://github.com/openprose/prose): the language spec, the skill, the examples, and Reactor
- [docs.prose.md](https://docs.prose.md): the documentation
- [prose.md](https://prose.md): OpenProse on the web

## About

OpenProse is built by OpenProse, Inc. The language is MIT licensed and will stay open.
