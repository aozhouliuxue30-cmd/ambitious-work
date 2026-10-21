# Get started in five minutes

[中文](QUICKSTART.md) | [English](QUICKSTART.en.md)

Version: 1.1.0 · AI 实干工作流 · Ambitious Work

## Option 1: Choose interface and output languages

1. Download `ambitious-work-bilingual-v1.1.0.html` from the release and open it in a browser, or open [docs/index.html](docs/index.html) in the full source package. GitHub's file preview cannot run it.
2. Choose a Chinese or English interface. Separately choose the deliverable language: 中文, English, or 中文 + English. Changing the interface does not change the deliverable language.
3. Enter your task, materials, constraints, and acceptance criteria. Generate the prompt, copy or download it, then paste it into your AI conversation.

The offline tool does not call a model, upload your inputs, or require a key. Inputs stay on the current page and may be lost on refresh or close. A generated prompt is not a completed task; run it in your AI product and check the result.

## Option 2: Copy a prompt directly

Copy “General entry point” in [PROMPTS.en.md](PROMPTS.en.md), or use the [Chinese TXT](examples/quick-prompt.txt) / [English TXT](examples/quick-prompt.en.txt). Replace bracketed fields. Specify `Output language: 中文`, `Output language: English`, or `Output language: 中文 + English`.

If no language is specified, the workflow follows your message language. Bilingual output should pair corresponding paragraphs and preserve the same numbers, citations, facts, and uncertainty. Interface and deliverable languages are independent. Without attachment or browsing features, paste relevant text into the conversation. Reading links and creating files depend on the AI product's actual capabilities.

## Option 3: Try a complete example

| Chinese example | English example | What to check |
| --- | --- | --- |
| [项目简报](examples/project-brief.md) | [Project brief](examples/project-brief.en.md) | Evidence labels, alternative explanations, unverified assumptions |
| [简历修改](examples/resume-review.md) | [Resume revision](examples/resume-review.en.md) | Real responsibilities, missing data, team boundaries |
| [学习小试验](examples/learning-experiment.md) | [Learning experiment](examples/learning-experiment.en.md) | A usable first version, bounded scope, stopping criteria |

All materials are explicitly fictional teaching examples. Expected outputs are acceptance guidance, not model evaluation scores. Replace them with your own non-sensitive materials and apply the same checks.

## Option 4: Import the standalone Skill

Download `ambitious-work-skill-v1.1.0.zip` from the [v1.1.0 release](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/tag/v1.1.0). Extract and retain the complete `ambitious-work/` directory, then follow your host's import instructions. Hosts supporting explicit invocation may use:

```text
Use $ambitious-work to complete my task:
Task: [Specific task]
Materials: [Supplied sources]
Constraints: [Requirements to preserve]
Acceptance criteria: [How to check completion]
Output language: [中文 / English / 中文 + English]
```

Invocation syntax and installation paths depend on the host. There is no installation script, automatic permission grant, or public one-click ChatGPT installation link.

## Check the first version

- If you requested a deliverable, confirm that it was produced.
- Check numbers, citations, dates, responsibilities, and completion status against the original materials.
- Uncertainty should remain visible; fluent wording cannot fill missing facts.
- In bilingual output, corresponding paragraphs must agree on facts, numbers, and qualifications.
- For files, measurements, and external actions, confirm that they actually occurred.
- If you only get a plan, ask: “Complete the first version possible with the existing materials and check it against my acceptance criteria.”

None of the 18 behavioral cases has been run as a model evaluation. The Skill cannot guarantee correctness or add capabilities absent from the host. See [validation notes](VALIDATION.md).
