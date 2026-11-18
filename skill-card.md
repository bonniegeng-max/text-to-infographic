## Description:

将文章/笔记/对话内容转化为结构化信息图 plan（JSON），经布局语义与数值一致性校验后，用内置渲染器产出自包含静态 HTML 信息图，可选导出 PNG（调用本机已有浏览器截图，不安装任何东西）。校验结果带稳定规则码机器回执（--json）、中文诊断（--explain）与严格模式（--fail-on-warn）。支持文本→plan 自动构建（analyze 布局推荐）、8 种风格 preset 与色彩 token；六种 chart_family 布局：飞轮/鱼骨/桑基/金字塔/时间线/仪表盘。仅在用户明确请求信息图时调用。

This skill is ready for commercial/non-commercial use.

## Publisher:

[bonniegeng-max](https://clawhub.ai/user/bonniegeng-max)

### License/Terms of Use:

MIT-0

## Use Case:

需要把对话、文章或笔记整理为单页信息图的用户和内容创作者，可在明确请求时使用此 skill 生成可编辑 plan、检查布局和数值，再导出静态 HTML 或 PNG。

### Deployment Geography for Use:

Global

## Known Risks and Mitigations:

Risk: Rendering overwrites an existing file at the selected output path.

Mitigation: Choose an unused output path or preserve the existing file before rendering.

Risk: Optional PNG export invokes a locally installed browser in headless mode to screenshot the generated HTML; it never downloads or installs software. Limited validation heuristics may miss inaccurate facts or numbers in a plan.

Mitigation: Review the plan against its source facts before sharing the infographic.

## Reference(s):

- [Text to Infographic on ClawHub](https://clawhub.ai/bonniegeng-max/skills/text-to-infographic)
- [Infographic plan schema](artifact/schemas/infographic-plan.schema.json)
- [Layout and fact validation rules](artifact/docs/校验规则规格-v0.1.md)

## Skill Output:

**Output Type(s):** [JSON, HTML, PNG, Validation report]

**Output Format:** [Structured infographic plan, validation findings with stable rule codes, a self-contained static HTML infographic, and an optional PNG rendered from the HTML via a locally installed browser (nothing is installed or downloaded).]

**Output Parameters:** [1D]

**Other Properties Related to Output:** [Supports six layouts: flywheel, fishbone, sankey, pyramid, timeline, and dashboard. The HTML uses inline CSS and SVG, with no JavaScript or external requests. The PNG export is optional and fails gracefully without affecting the HTML output.]

## Skill Version(s):

1.4.0 (source: frontmatter and release evidence)

## Ethical Considerations:

Users should evaluate whether this skill is appropriate for their environment, review any generated or modified files before relying on them, and apply their organization's safety, security, and compliance requirements before deployment.
