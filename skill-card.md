## Description:

Turns content supplied in the current conversation into a structured, single-page infographic specification and, when explicitly requested, copyable standalone HTML source.

This skill is ready for commercial/non-commercial use.

## Publisher:

[bonniegeng-max](https://clawhub.ai/user/bonniegeng-max)

### License/Terms of Use:

MIT-0

## Use Case:

Use this skill to define a reviewable one-page information hierarchy before visual design, or to represent supplied content as a self-contained static HTML document. It maps communication objectives, reading order, sections, content blocks, visual forms, layout, typography, accessibility treatment, and supplied source notes without adding facts.

Best-fit requests include:

- “Turn these notes into a one-page infographic specification.”
- “Create standalone HTML for this infographic.”
- “Organize this supplied comparison into an infographic layout.”

This version works only with content already available in the current conversation. It does not research, enrich, fetch, execute scripts, render or create files, upload, publish, or modify external state.

### Deployment Geography for Use:

Global

## Known Risks and Mitigations:

Risk: Generated infographic copy or HTML could still present supplied content inaccurately or with poor layout choices.

Mitigation: Review the generated output for factual accuracy, source traceability, and presentation quality before publishing or sharing it.

Risk: Users may expect enrichment, citations, or assets that are not present in the conversation.

Mitigation: Keep missing facts, values, citations, assets, and preferences unspecified unless the user supplies them.

Risk: Users may interpret standalone HTML source as a rendered or saved deliverable.

Mitigation: State that v1.1.3 returns copyable source only. The HTML uses inline CSS, has no active behavior or external dependencies, and must be reviewed before use.

## Reference(s):

- [ClawHub skill page](https://clawhub.ai/bonniegeng-max/text-to-infographic)
- [README](README.md)
- [Skill definition](SKILL.md)
- [FAQ](docs/faq.md)
- [Canonical cases](docs/canonical-cases.md)
- [GEO evaluation](docs/geo-evaluation.md)

## Skill Output:

**Output Type(s):** [text, markdown, code]

**Output Format:** [Markdown containing a one-page infographic specification and, when explicitly requested, a complete standalone HTML document with inline CSS]

**Output Parameters:** [1D]

**Other Properties Related to Output:** [Current-conversation content only; one page; static and self-contained; semantic text; no active behavior, external dependencies, file writes, or state changes]

## Skill Version(s):

1.1.3 (source: frontmatter and server release evidence)

## Ethical Considerations:

Users should evaluate whether this skill is appropriate for their environment, review any generated or modified files before relying on them, and apply their organization's safety, security, and compliance requirements before deployment.
