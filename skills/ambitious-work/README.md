# AI 实干工作流 · Ambitious Work

[中文](README.md) | [English](README.en.md)

入口：[SKILL.md](SKILL.md)。版本：1.1.0。标识：`ambitious-work`；“野心工作法”保留为调用别名。

把研究、作品集、求职和项目任务推进到可检查成品，支持中文、English 与中英双语。导入支持 Agent Skills 的工具后，按宿主的调用方式选择本技能；支持显式调用时可使用：

```text
请使用 $ambitious-work 处理下面的任务。
任务：【具体成品与使用者】
材料：【粘贴内容或提供附件】
限制：【事实、范围、格式与不能做的事】
验收：【完成标准】
输出语言：【中文 / English / 中英双语】
先读取实际材料，完成当前可做的第一版，再对照要求检查。
不要只给计划，不编造经历、数据、引用或测试结果。
```

明确语言要求优先；未指定时跟随用户消息语言。双语逐段对应，数字、引用、事实与不确定性保持一致。界面语言和成品语言独立。

保留整个目录与相对引用的资源；安装路径和导入方式由宿主决定，复制文件不等于已经安装或启用。独立 Skill 不含插件清单和离线 HTML 工具；离线工具在完整源码包中。

详细方法在 [playbook.md](references/playbook.md)，应用配方在 [applications.md](references/applications.md)，来源及主题覆盖在 [sources.md](references/sources.md)。提示词在 [prompts.md](assets/prompts.md)，早期独立提示词在 [prior-prompts.md](assets/prior-prompts.md)。详细参考材料以中文保留，不影响按用户要求输出其他语言。公开版不含精读 PDF。

[evals/test-cases.json](evals/test-cases.json) 共 18 个用例：原 15 个保留，1.1.0 新增 3 个语言用例。所有用例均未运行模型行为评测；不是测试通过报告。见 [VALIDATION.md](VALIDATION.md)。

没有预设外部账号、MCP 服务器、后台任务或软件安装动作；技能不能凭空获得工具和权限。

独立实现采用 [MIT License](LICENSE)，来源及第三方权利边界见 [NOTICE.md](NOTICE.md)。
