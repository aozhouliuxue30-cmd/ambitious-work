# AI 实干工作流 · Ambitious Work

**让 AI 读取材料、做出成品，再检查它是否满足要求。**

这是一个中文 AI 工作流、提示词和 Skill 开源项目。适合把研究资料整理成有出处的简报，把项目记录整理成作品集初稿，或依据真实经历改进求职材料。版本 **1.0.2**，项目标识 `ambitious-work`；原名称“野心工作法”保留为调用别名。

## 先用起来：不需要安装

把下面整段复制到你正在使用的 AI 对话，再填入任务和材料即可：

```text
请按“AI 实干工作流”完成下面的任务。

任务：[我要交付的具体成品，以及给谁使用]
材料：[粘贴资料；或附上文件并指出要读哪些]
限制：[必须保留的事实、范围、格式和不能做的事]
完成标准：[怎样检查成品可以使用]

先读取已提供的材料，区分事实、推测与缺失信息。目标明确就开始，
不要只给计划；把当前条件下能完成的部分做成第一版。
保留我的原始要求，不编造经历、数据、引用或测试结果。
对照完成标准检查第一版，修正可修正的问题。
先交成品，再简要标明实际检查了什么、还有什么没有验证。
如果缺少必要工具或资料，明确指出，并继续完成不依赖它们的部分。
外部发布、发送、付费或删除，按我的明确授权和工具确认规则执行。
```

普通对话可以使用这个提示词；联网、读附件、制作文件等操作取决于你所用产品的实际能力。提示词不会自动开通工具、安装插件或取得账号权限。

想用一个有完整输入的例子试试，打开 [快速开始](QUICKSTART.md) 或 [示例目录](examples/README.md)。

## 能帮你做什么

| 你已有的东西 | 交给 AI 的任务 | 应检查的成品 |
| --- | --- | --- |
| 项目笔记、用户反馈、访谈片段 | 整理项目问题、证据、方案和待验证项 | 带证据位置的项目简报或作品集初稿 |
| 真实简历与目标岗位要求 | 找匹配点和缺口，修改现有经历表达 | 保留事实、不填造数字的简历修改稿 |
| 多篇资料或研究记录 | 比较观点、整理支持与反例 | 可追溯来源并标明不确定性的研究简报 |
| 一个模糊的学习或项目想法 | 做一个范围可控的小试验 | 有输入、产出与检查标准的第一版 |

它是一套让模型做事的规则，不是能够独立运行的应用。简单翻译、局部润色和一句话问答直接完成，不必套用整套流程。

## 选择你需要的下载

进入 [v1.0.2 发布页](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/tag/v1.0.2)：

| 下载 | 内容 | 适合谁 |
| --- | --- | --- |
| [完整源码 ZIP](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.0.2/ambitious-work-v1.0.2.zip) | 两份插件清单、完整 Skill、提示词、示例、许可和来源说明 | 想保存完整源码或自行创建插件的用户 |
| [独立 Skill ZIP](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.0.2/ambitious-work-skill-v1.0.2.zip) | 独立 `ambitious-work/` Skill 目录及所需参考文件 | 使用支持 Agent Skills 的工具的用户 |
| [入门提示词 TXT](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/download/v1.0.2/start-here-v1.0.2.txt) | 可复制的通用入门提示词，附许可与来源 | 想立即在普通对话中使用的用户 |

也可直接浏览 [完整源码](https://github.com/aozhouliuxue30-cmd/ambitious-work)、[独立 Skill](skills/ambitious-work/README.md) 或 [提示词文件](PROMPTS.md)，不依赖下载附件。

下载包本身不会安装。不同产品是否支持导入 Skill 或创建插件，以该产品当前界面和说明为准；本仓库没有公共 ChatGPT 一键安装入口，也不表示它已在任何账号启用。

## 给 Skill 和插件用户

完整 Skill 入口是 [skills/ambitious-work/SKILL.md](skills/ambitious-work/SKILL.md)。请保留整个目录，避免丢失其相对引用的参考材料、许可和来源说明。导入支持该格式的宿主后，可使用 `$ambitious-work`，或按该宿主的调用方式选择本技能。

`plugin.json` 和 `.codex-plugin/plugin.json` 是插件源码及兼容清单。它们供支持相应格式的工具使用；创建、导入、安装、启用和本次对话已加载是不同状态。普通用户无需处理这些文件，先复制上方提示词即可。

## 验证状态

1.0.2 更新展示名称与使用说明，新增入门提示词、三个可复制示例和下载说明；技能执行规则保持原有逻辑。已执行的结构、格式、链接和内容检查记录在 [VALIDATION.md](VALIDATION.md)。

原有 15 个行为用例已编写，**1.0.1 与 1.0.2 均未运行模型行为评测**；示例中的“预期输出”用于理解格式，并非模型已经通过测试的记录。本项目不声称已证明效率、准确率或任务成功率提升。实际成品仍须按任务材料检查。

## 来源与许可

本项目参考 Felix Rieseberg 的 [How to be more ambitious: A tutorial for humans with models](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/) 及项目早期整理材料，独立编写工作流、提示词、示例和行为用例，制作过程使用了 AI 辅助。它不是原作者或 Anthropic 的官方产品、全文转载或授权译本。详细归因见 [NOTICE.md](NOTICE.md) 和 [来源索引](skills/ambitious-work/references/sources.md)。

独立实现采用 [MIT License](LICENSE)，署名使用 GitHub 用户名 `aozhouliuxue30-cmd`。保留许可和版权声明即可使用、修改、分发及商用；第三方文章、图片和外链论文不属于该授权范围。公开包不含文章全文、完整翻译、原图或精读 PDF。
