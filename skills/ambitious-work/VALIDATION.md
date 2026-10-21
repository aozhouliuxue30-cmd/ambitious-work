# 独立 Skill 校验记录 / Standalone Skill validation

版本 / Version：1.1.0。日期 / Date：2026-10-21。

## 实际执行 / Checks performed

- SKILL.md frontmatter 与 agents/openai.yaml 通过 Ruby Psych.safe_load 安全解析，技能标识为 ambitious-work，版本为 1.1.0，语言元数据为 zh-CN,en。
- 显示名称保留“AI 实干工作流 · Ambitious Work”，原名称“野心工作法”仍为调用别名；agent default_prompt 的实际字符串与 1.0.2 相同。
- Skill 执行主体与 1.0.2 比较，除新增“语言选择”章节外逐字一致；语言规则覆盖明确要求、默认跟随用户消息、双语逐段对应与界面 / 成品语言独立。
- evals/test-cases.json 可解析，18 个用例标识唯一；原 15 个用例内容与 1.0.2 一致，新增 3 个语言用例。
- 相对链接存在且位于发布目录内；文本模式扫描未检出邮箱、私有插件 ID、本机用户目录路径、常见令牌格式或私钥头。模式扫描不保证发现所有敏感内容。
- 技能目录不含 PDF、图片、执行脚本或符号链接；LICENSE 与 NOTICE.md 和 1.0.2 字节一致。

YAML parses safely. The Skill identity, version, display name, and preserved default prompt are consistent. Apart from the added language-selection section, the execution body is identical to 1.0.2. All 18 case identifiers are unique; the original 15 cases are unchanged. Local links resolve within the package, targeted sensitive-text patterns found no matches, and license and attribution notices are unchanged.

## 未执行与范围 / Not verified and scope

所有 18 个用例均未运行模型行为评测；未执行宿主导入、安装、启用或长期使用验证。用例不是测试通过报告，不证明模型一定遵从语言要求，也不证明效率或成功率提升。

此检查只针对发布文件，不审计 Git 提交历史、远端缓存、其他副本或账号设置，不宣称历史邮箱已清除或安全漏洞已修复。安装和调用状态以宿主回执为准。独立 Skill 包不含离线 HTML 工具，浏览器交互不属于本目录检查范围。

None of the 18 cases has been run as a model evaluation. No host import, installation, enablement, long-term use, or effectiveness has been verified. This file-level check does not audit Git history, caches, other copies, or account settings. The standalone Skill does not include the offline HTML tool.
