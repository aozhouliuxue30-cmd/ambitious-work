# AI 实干工作流 · Ambitious Work

**[中文](README.md) | [English](README.en.md)**

**Ask AI to read the materials, make the deliverable, and check it against your requirements.**

An open-source workflow, prompt collection, and Skill supporting Chinese, English, and paired Chinese–English output. Use it for research briefs, project portfolios, job application materials, and small learning experiments. Version **1.1.0**, identifier `ambitious-work`; the original Chinese name “野心工作法” remains an invocation alias.

## Start using it

Open the [bilingual prompt tool](docs/index.html). Switch the interface between 中文 and English, then independently select the deliverable language: **中文, English, or 中文 + English**. Fill in the task, materials, constraints, and acceptance criteria. Generate, copy, or download the prompt, then paste it into your AI conversation.

GitHub's file preview does not run HTML. Download the [standalone offline HTML tool](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/ambitious-work-bilingual-v1.1.0.html) or full source package and open the local file in your browser. The tool does not call a model, upload your inputs, or require an API key. Form text stays on the current page and may be lost on refresh or close; download it if you need to keep it. How an external AI product handles content you later paste there depends on that product's settings.

You can also copy this prompt directly, with no installation:

```text
Use the Ambitious Work workflow to complete the task below.

Task: [The specific deliverable and who will use it]
Materials: [Paste sources, or attach files and identify what to read]
Constraints: [Facts, scope, format, and actions that must be preserved or avoided]
Acceptance criteria: [How to check whether the deliverable is usable]
Output language: [中文 / English / 中文 + English]

Read the supplied materials first. Separate facts, assumptions, and missing information.
When the goal is clear, start work and produce the first version possible with the
available inputs; do not stop at a plan.
Preserve my original requirements. Do not invent experience, data, citations, or test results.
Check the first version against the acceptance criteria and fix what can be fixed.
Deliver the artifact first, then briefly state what was actually checked and what remains unverified.
Follow an explicit language choice; otherwise follow the language of my message.
For bilingual output, pair Chinese and English paragraph by paragraph, keeping numbers,
citations, facts, and uncertainty consistent. Interface language and deliverable language
are independent; the output language selected here controls the deliverable.
If necessary tools or materials are missing, explain the gap and complete the work that
does not depend on it.
For external publishing, sending, payments, or deletion, follow my explicit authorization
and the host tool's confirmation rules.
```

Reading attachments, browsing, and creating files depend on your AI product's actual capabilities. A prompt does not enable tools, install a plugin, or grant account permissions. An explicit language request takes precedence; otherwise the workflow follows your message language. Bilingual deliverables pair corresponding paragraphs and keep numbers, citations, facts, and uncertainty consistent.

For complete sample inputs, see [Quick start](QUICKSTART.en.md), [Prompts](PROMPTS.en.md), and [Examples](examples/README.en.md). Chinese versions: [快速开始](QUICKSTART.md), [提示词](PROMPTS.md), [示例](examples/README.md).

## What it helps you make

| Your inputs | The AI task | What to check |
| --- | --- | --- |
| Project notes, feedback, interview excerpts | Organize the problem, evidence, options, and open questions | A project brief or portfolio draft with traceable evidence |
| Your real resume and target job requirements | Identify matches and gaps, then improve the wording | A revision that preserves facts and invents no metrics |
| Multiple sources or research notes | Compare claims, supporting evidence, and counterexamples | A sourced brief with uncertainty made explicit |
| An early learning or project idea | Run a small, bounded experiment | A first version with inputs, outputs, and acceptance criteria |

Use the workflow inside an AI product; the offline tool prepares and exports prompts. Simple translations, small edits, and one-sentence questions should be completed directly without the full workflow.

## Downloads and formats

Visit the [v1.1.0 release](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/tag/v1.1.0):

| Download | Contents | Best for |
| --- | --- | --- |
| [Offline bilingual HTML tool](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/ambitious-work-bilingual-v1.1.0.html) | Chinese / English interface, three output-language options, prompt generation, copy, and download | Choosing a language and getting started |
| [Chinese starter prompt TXT](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/start-here-zh-v1.1.0.txt) | Copyable Chinese template, license, and attribution | Any AI conversation |
| [English starter prompt TXT](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/start-here-en-v1.1.0.txt) | Copyable English template, license, and attribution | English-language users |
| [Standalone Skill ZIP](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/ambitious-work-skill-v1.1.0.zip) | Complete `ambitious-work/` directory and referenced resources | Hosts that support Agent Skills |
| [Full source ZIP](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/ambitious-work-v1.1.0.zip) | Offline tool, bilingual guides, examples, two manifests, Skill, license, and attribution | Saving or modifying the full source |

You can also browse the [source repository](https://github.com/aozhouliuxue30-cmd/ambitious-work), [Skill guide](skills/ambitious-work/README.en.md), [Chinese prompt TXT](examples/quick-prompt.txt), or [English prompt TXT](examples/quick-prompt.en.txt). Downloading does not install anything. Skill or plugin import depends on the host's current capabilities and instructions. This repository has no public one-click ChatGPT installation link and does not imply that a plugin is enabled in any account.

## Skill and plugin users

The Skill entry point is [skills/ambitious-work/SKILL.md](skills/ambitious-work/SKILL.md). Keep the entire directory so referenced resources, license, and attribution remain available. Hosts supporting explicit invocation may use `$ambitious-work`, with `Output language: 中文 / English / 中文 + English`.

`plugin.json` and `.codex-plugin/plugin.json` are source and compatibility manifests. Creation, import, installation, enablement, and loading in a conversation are distinct states. Interface language changes the offline tool's labels; the output-language setting or your explicit instruction controls the deliverable language. Detailed Skill references remain in Chinese; the execution rules support responses in the requested language.

## Validation status

Version 1.1.0 adds the bilingual prompt tool, Chinese and English guides and examples, and explicit language-selection rules. Existing execution rules and the original 15 behavioral cases are preserved; 3 language cases bring the total to 18. **None of the behavioral cases has been run as a model evaluation.** Example “expected outputs” describe acceptance criteria, not passing test results. See [VALIDATION.md](VALIDATION.md) for checks and limits. No efficiency, accuracy, or task-success improvement has been demonstrated.

## Attribution and license

This independent workflow draws on Felix Rieseberg's [How to be more ambitious: A tutorial for humans with models](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/) and early project notes. Prompts, examples, and behavioral cases were written independently with AI assistance. This is not an official product of the author or Anthropic, a full reproduction, or an authorized translation. See [NOTICE.md](NOTICE.md) and the [source index](skills/ambitious-work/references/sources.md).

The independent implementation uses the [MIT License](LICENSE), credited to the GitHub username `aozhouliuxue30-cmd`. Use, modify, distribute, and commercialize it while retaining the license and copyright notice. Third-party articles, images, and linked papers are outside that grant. The public package contains no full article, full translation, original images, or close-reading PDF.
