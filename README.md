# 野心工作法 · 个人 Skill

版本：1.0.1。标识：`ambitious-work`。整理日期：2026-10-21。

## 用来做什么

对研究、设计、作品集、求职材料和项目探索，先确认目标与边界，再实际读取资料、选择方法、制作成果和检验。简单问题不会被强行扩成大项目。

本文档包是可复用的技能实现，不是文章全文或官方译本。方法主题、案例定位与来源见 `skills/ambitious-work/references/sources.md`。原文背景故事保留索引，操作规则另行编写。

## 在 ChatGPT 中使用

这是插件源码，不是会自动安装到账号的程序。已有账号内插件的用户可打开其详情页，按实际页面完成安装；使用本源码的用户需先通过 Plugin Creator 创建自己的插件。是否提供安装按钮及如何启用，以宿主界面为准。新对话中选择“野心工作法”，再发具体任务。源码公开、插件创建、账号安装和当前会话加载是不同状态。

示例：

> 用野心工作法完成这个作品集项目。先核对我的实际资料，保留要求，完成能交付的第一版并检查，不要只给计划。

插件只有技能和本地参考材料，没有外部服务器、账号凭据、后台任务或自动安装脚本。需要联网、文件处理或其他工具时，使用所在会话实际提供的能力和授权。

宿主使用方式参考：https://help.openai.com/en/articles/20001256-plugins-in-chatgpt

## 文件结构

```text
plugin.json
.codex-plugin/plugin.json
README.md
LICENSE
NOTICE.md
CHANGELOG.md
VALIDATION.md
skills/ambitious-work/
  SKILL.md
  agents/openai.yaml
  references/
    playbook.md
    applications.md
    sources.md
  assets/
    prompts.md
    task-brief.md
    prior-prompts.md
  evals/test-cases.json
```

## 独立 Skill 包

单独使用技能时，保留 `skills/ambitious-work/` 的完整目录，包括 LICENSE、NOTICE.md 和相对引用的资源。该目录不带插件清单；是否可直接导入由目标工具决定。不要将“已生成文件”误认为“已安装到另一款产品”。

格式参考：https://agentskills.io/specification

## 验证说明

本版本已检查包内结构、相对链接、JSON/YAML、版本一致性和已知个人联系信息；记录见 VALIDATION.md。这些是静态检查，不是宿主安装验证。行为用例已编写，但未在不同模型上执行，不声称已证明效果提升。输出是否正确仍需依靠实际任务中的资料与检验。

## 归因

参考 Felix Rieseberg 的 How to be more ambitious: A tutorial for humans with models，以及项目早期整理的中文精读与提示词。新增工作流、例子、权限规则与测试均为本次独立编写；不是作者或 Anthropic 的官方产品。原文和外链论文不重新打包。

## 开源许可

独立编写的工作流、提示词、应用配方、测试与配套文档采用 MIT 许可证，署名使用 GitHub 用户名 `aozhouliuxue30-cmd`。许可全文见 [LICENSE](LICENSE)，第三方内容边界见 [NOTICE.md](NOTICE.md)。MIT 允许在保留许可与版权声明的条件下使用、修改、分发及商用。

原文章全文、完整翻译、原图、外链论文与精读 PDF 均未收入公开版。来源链接与独立实现不能当成原作者授权或背书。

本包没有外部服务器、自动执行钩子、账户凭据或后台调度。
