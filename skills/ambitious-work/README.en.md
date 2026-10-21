# AI 实干工作流 · Ambitious Work

[中文](README.md) | [English](README.en.md)

Entry point: [SKILL.md](SKILL.md). Version: 1.1.0. Identifier: `ambitious-work`; the original Chinese name “野心工作法” remains an invocation alias.

Turn research, portfolio, job application, and project tasks into checkable deliverables in Chinese, English, or paired Chinese–English output. Import the Skill into a host supporting Agent Skills and follow that host's invocation method. With explicit invocation support:

```text
Use $ambitious-work to complete this task.
Task: [Specific deliverable and audience]
Materials: [Paste content or attach files]
Constraints: [Facts, scope, format, and actions to avoid]
Acceptance criteria: [How to check completion]
Output language: [中文 / English / 中文 + English]
Read the actual materials, make the first version possible, and check it against the requirements.
Do not stop at a plan or invent experience, data, citations, or test results.
```

Explicit language requests take precedence. Otherwise follow the user's message language. Bilingual output pairs corresponding paragraphs with consistent numbers, citations, facts, and uncertainty. Interface and deliverable languages are independent.

Keep the whole directory and its relative resources. Installation paths and import methods depend on the host; copying files does not establish installation or enablement. The standalone Skill contains no plugin manifest or offline HTML tool. The offline tool is in the full source package.

Detailed methods are in [playbook.md](references/playbook.md), task recipes in [applications.md](references/applications.md), and attribution and topic coverage in [sources.md](references/sources.md). Prompts are in [prompts.md](assets/prompts.md), with earlier independent prompts in [prior-prompts.md](assets/prior-prompts.md). Detailed references remain in Chinese; requested output languages are supported. The public package excludes the close-reading PDF.

[evals/test-cases.json](evals/test-cases.json) contains 18 authored cases: the original 15 and 3 language cases added in 1.1.0. None has been run as a model evaluation. This is not a passing-test report; see [VALIDATION.md](VALIDATION.md).

There are no preconfigured external accounts, MCP servers, background tasks, or software-installation actions. The Skill cannot grant itself tools or permissions.

The independent implementation uses the [MIT License](LICENSE). See [NOTICE.md](NOTICE.md) for attribution and third-party rights.
