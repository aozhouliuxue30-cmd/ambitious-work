# 五分钟开始使用

[中文](QUICKSTART.md) | [English](QUICKSTART.en.md)

版本：1.1.0 · AI 实干工作流 · Ambitious Work

## 方式一：选择界面和输出语言

1. 下载发布页的 `ambitious-work-bilingual-v1.1.0.html`，用浏览器打开，或打开完整源码中的 [docs/index.html](docs/index.html)。GitHub 文件预览不能运行这个工具。
2. 选择中文或 English 界面。再单独选择成品输出语言：中文、English 或中英双语；切换界面不会替你改变成品语言。
3. 填写任务、材料、限制和完成标准，生成提示词，复制或下载后粘贴到你的 AI 对话。

这个离线工具不调用模型、不上传输入、不需要密钥。输入留在当前页面，刷新或关闭可能丢失。生成提示词不等于任务已完成，还需在 AI 产品中执行并核对结果。

## 方式二：直接复制提示词

复制 [PROMPTS.md](PROMPTS.md) 的“通用入口”，或使用 [中文 TXT](examples/quick-prompt.txt) / [English TXT](examples/quick-prompt.en.txt)，替换方括号后发送。可以直接写：`输出语言：中文`、`Output language: English` 或 `输出语言：中英双语`。

未指定时跟随用户消息语言。双语输出应逐段对应，数字、引用、事实和不确定性一致。界面语言与成品语言独立。无附件或联网功能时，把相关文字粘贴到对话；读取链接或制作文件依赖 AI 产品的实际功能。

## 方式三：用完整例子练习

| 中文例子 | English example | 检查重点 |
| --- | --- | --- |
| [项目简报](examples/project-brief.md) | [Project brief](examples/project-brief.en.md) | 证据编号、替代解释、未验证假设 |
| [简历修改](examples/resume-review.md) | [Resume revision](examples/resume-review.en.md) | 职责真实、缺失数据、团队边界 |
| [学习小试验](examples/learning-experiment.md) | [Learning experiment](examples/learning-experiment.en.md) | 可检查的成品、有限范围、停止条件 |

资料均为明确标注的虚构教学材料。预期输出是验收说明，不是模型评测成绩。可以换成自己的非敏感资料，再用同样的方法检查。

## 方式四：导入独立 Skill

从 [v1.1.0 发布页](https://github.com/aozhouliuxue30-cmd/ambitious-work/releases/tag/v1.1.0) 下载 `ambitious-work-skill-v1.1.0.zip`。解压并保留 `ambitious-work/` 的完整内容，按宿主的导入说明操作。支持显式调用的宿主可使用：

```text
请使用 $ambitious-work 完成我的任务：
任务：【具体任务】
材料：【提供的材料】
限制：【必须保留的要求】
验收：【完成标准】
输出语言：【中文 / English / 中英双语】
```

调用语法和安装目录由宿主决定。没有安装脚本，不会替你打开权限，也没有公共 ChatGPT 一键安装链接。

## 检查第一版是否可用

- 有指定交付物时，先看是否交出成品。
- 按原始材料核对数字、引用、日期、职责与完成状态。
- 不确定判断应标明，缺少事实不能用流畅表述补足。
- 双语逐段对应，两种语言的事实、数字与限定应一致。
- 需要文件、实测或外部操作时，核对是否真的发生。
- 若只拿到计划，可追问：“请用现有材料完成不依赖缺口的第一版，并对照验收标准检查。”

18 个行为用例均未运行模型行为评测；技能不能保证正确或增加宿主没有的能力。见 [验证记录](VALIDATION.md)。
