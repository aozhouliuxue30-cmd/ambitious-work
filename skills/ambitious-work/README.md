# AI 实干工作流 · Ambitious Work

入口：[SKILL.md](SKILL.md)。版本：1.0.2。标识：`ambitious-work`；原名称“野心工作法”仍可作为调用别名。

这是一套把研究、作品集、求职和项目任务推进到可检查成品的中文工作流。导入支持 Agent Skills 的工具后，可按宿主的调用方式选择本技能；支持显式调用时可使用：

```text
请使用 $ambitious-work 处理下面的任务。
任务：【具体成品与使用者】
材料：【粘贴内容或提供附件】
限制：【事实、范围、格式与不能做的事】
验收：【完成标准】
先读取实际材料，完成当前可做的第一版，再对照要求检查。
不要只给计划，不编造经历、数据、引用或测试结果。
```

本目录遵循 Agent Skills 的基础结构。请保留整个目录和相对引用的资源；安装路径和导入方式由宿主决定，复制文件不等于已经安装或启用。独立 Skill 不带插件清单。

详细方法在 [playbook.md](references/playbook.md)，应用配方在 [applications.md](references/applications.md)，来源及主题覆盖在 [sources.md](references/sources.md)。可复制的更多提示词在 [prompts.md](assets/prompts.md)。项目早期的独立提示词在 [prior-prompts.md](assets/prior-prompts.md)，公开版不包含精读 PDF。

[evals/test-cases.json](evals/test-cases.json) 的 15 个行为用例在 1.0.1 与 1.0.2 均未运行；它们不是测试通过报告。验证范围见 [VALIDATION.md](VALIDATION.md)。

没有预设外部账号、MCP 服务器、后台任务或软件安装动作。技能不能凭空获得工具和权限。

本目录的独立实现采用 [MIT License](LICENSE)。来源及第三方权利边界见 [NOTICE.md](NOTICE.md)。
