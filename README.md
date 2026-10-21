# AI 实干工作流 · Ambitious Work

**[中文](README.md) | [English](README.en.md)**

**让 AI 读取材料、做出成品，再检查它是否满足要求。**

这是一个支持中文、English 与中英双语输出的 AI 工作流、提示词和 Skill 开源项目。适合研究简报、项目作品集、求职材料和小型学习试验。版本 **1.1.0**，标识 `ambitious-work`；“野心工作法”保留为调用别名。

## 先用起来

打开 [双语提示词工具](docs/index.html)，切换中文或 English 界面，再独立选择成品输出语言：**中文、English、中英双语**。填写任务、材料、限制和完成标准后，可以生成、复制或下载提示词，再粘贴到你使用的 AI 对话。

在 GitHub 文件预览里不能运行 HTML。请下载 [离线工具 HTML](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/ambitious-work-bilingual-v1.1.0.html) 或完整源码包后，用浏览器打开本机文件。工具不调用模型、不上传输入、不需要密钥；表单文本留在当前页面，刷新或关闭可能丢失，请按需下载保存。外部 AI 产品如何处理你随后粘贴的内容，取决于该产品的设置。

也可以直接复制下面的提示词，无需安装：

```text
请按“AI 实干工作流”完成下面的任务。

任务：[我要交付的具体成品，以及给谁使用]
材料：[粘贴资料；或附上文件并指出要读哪些]
限制：[必须保留的事实、范围、格式和不能做的事]
完成标准：[怎样检查成品可以使用]
输出语言：[中文 / English / 中英双语]

先读取已提供的材料，区分事实、推测与缺失信息。目标明确就开始，
不要只给计划；把当前条件下能完成的部分做成第一版。
保留我的原始要求，不编造经历、数据、引用或测试结果。
对照完成标准检查第一版，修正可修正的问题。
先交成品，再简要标明实际检查了什么、还有什么没有验证。
明确指定语言时按要求输出；未指定时跟随我的消息语言。
中英双语时逐段对应，确保数字、引用、事实与不确定性一致。
界面语言和成品语言独立，以这里的输出语言要求为准。
如果缺少必要工具或资料，明确指出，并继续完成不依赖它们的部分。
外部发布、发送、付费或删除，按我的明确授权和工具确认规则执行。
```

读附件、联网和制作文件取决于 AI 产品的实际能力。提示词不会开通工具、安装插件或取得账号权限。明确语言要求优先；未指定时跟随用户消息语言。中英双语成品逐段对应，数字、引用、事实和不确定性应保持一致。

想用完整输入练习，打开 [快速开始](QUICKSTART.md)、[提示词](PROMPTS.md) 或 [示例目录](examples/README.md)。英文版分别为 [Quick start](QUICKSTART.en.md)、[Prompts](PROMPTS.en.md) 和 [Examples](examples/README.en.md)。

## 能帮你做什么

| 你已有的东西 | 交给 AI 的任务 | 应检查的成品 |
| --- | --- | --- |
| 项目笔记、用户反馈、访谈片段 | 整理项目问题、证据、方案和待验证项 | 带证据位置的项目简报或作品集初稿 |
| 真实简历与目标岗位要求 | 找匹配点和缺口，修改现有经历表达 | 保留事实、不填造数字的简历修改稿 |
| 多篇资料或研究记录 | 比较观点、整理支持与反例 | 可追溯来源并标明不确定性的研究简报 |
| 一个模糊的学习或项目想法 | 做一个范围可控的小试验 | 有输入、产出与检查标准的第一版 |

工作流需要在 AI 产品中使用；离线工具只帮你整理并导出提示词。简单翻译、局部润色和一句话问答直接完成，不必套用整套流程。

## 下载与使用方式

进入 [v1.1.0 发布页](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/tag/v1.1.0)：

| 下载 | 内容 | 适合谁 |
| --- | --- | --- |
| [双语离线工具 HTML](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/ambitious-work-bilingual-v1.1.0.html) | 中文 / English 界面切换，三种输出语言，表单生成、复制和下载提示词 | 想调整语言后立即使用的人 |
| [中文入门提示词 TXT](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/start-here-zh-v1.1.0.txt) | 可复制中文模板，附许可与来源 | 普通 AI 对话用户 |
| [English starter prompt TXT](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/start-here-en-v1.1.0.txt) | 可复制英文模板，附许可与来源 | 使用英文的用户 |
| [独立 Skill ZIP](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/ambitious-work-skill-v1.1.0.zip) | 完整 `ambitious-work/` Skill 目录与相对引用资源 | 使用支持 Agent Skills 的工具的用户 |
| [完整源码 ZIP](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.1.0/ambitious-work-v1.1.0.zip) | 离线工具、双语指南、示例、两份清单、Skill、许可与来源 | 想保存或修改完整源码的人 |

也可直接浏览 [完整源码](https://github.com/aozhouliuxue30-cmd/ambitious-work)、[独立 Skill](skills/ambitious-work/README.md)、[中文提示词 TXT](examples/quick-prompt.txt) 或 [English prompt TXT](examples/quick-prompt.en.txt)。下载包不会自动安装；是否支持导入 Skill 或插件，以宿主产品当前界面和说明为准。本仓库没有公共 ChatGPT 一键安装入口，也不表示插件已在任何账号启用。

## 给 Skill 和插件用户

Skill 入口是 [skills/ambitious-work/SKILL.md](skills/ambitious-work/SKILL.md)。保留整个目录，避免丢失参考材料、许可与来源。支持显式调用的宿主可使用 `$ambitious-work`，并写明 `输出语言：中文 / English / 中英双语`。

`plugin.json` 和 `.codex-plugin/plugin.json` 是插件源码及兼容清单。创建、导入、安装、启用和当前对话已加载是不同状态。界面语言只影响离线工具的显示；成品语言由输出语言选项或你的明确指令决定。

## 验证状态

1.1.0 新增双语提示词工具、中英文指南与示例，并补充 Skill 的语言选择规则。原有执行规则保持，15 个原行为用例内容保持，新增 3 个语言用例，共 18 个。**所有行为用例均未运行模型行为评测**；示例“预期输出”是验收说明，不是测试通过记录。已执行的检查与未验证范围见 [VALIDATION.md](VALIDATION.md)。本项目不声称已证明效率、准确率或任务成功率提升。

## 来源与许可

本项目参考 Felix Rieseberg 的 [How to be more ambitious: A tutorial for humans with models](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/) 及项目早期整理材料，独立编写工作流、提示词、示例和行为用例，制作过程使用了 AI 辅助。它不是原作者或 Anthropic 的官方产品、全文转载或授权译本。详细归因见 [NOTICE.md](NOTICE.md) 和 [来源索引](skills/ambitious-work/references/sources.md)。

独立实现采用 [MIT License](LICENSE)，署名为 GitHub 用户名 `aozhouliuxue30-cmd`。保留许可和版权声明即可使用、修改、分发及商用；第三方文章、图片和外链论文不属于该授权范围。公开包不含文章全文、完整翻译、原图或精读 PDF。
