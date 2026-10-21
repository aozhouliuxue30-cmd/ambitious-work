# 1.1.0 校验记录 / Validation notes

版本 / Version：1.1.0。日期 / Date：2026-10-21。

## 文档、清单与 Skill：实际执行 / Checks performed

- 37 个文档、清单与 Skill 发布文件可按 UTF-8 读取；此计数不含 `docs/` 离线工具。未发现符号链接、PDF、图片或独立执行脚本。
- 两个插件清单与行为用例 JSON 可解析。Skill frontmatter 与 agents/openai.yaml 使用 Ruby Psych.safe_load 安全解析；未安装额外依赖。
- 两个清单、Skill 元数据和行为用例版本为 1.1.0；标识为 ambitious-work。两个清单的展示配置一致，显示名称保留“AI 实干工作流 · Ambitious Work”，短描述在 30 字符以内。
- 两个插件清单的 defaultPrompt 原值、类型与顺序保留；Skill agent 的 default_prompt 原值保留。
- 18 个行为用例标识唯一；前 15 个用例与 1.0.2 的内容完全一致，新写 3 个语言用例。用例文件状态仍为“已编写、未运行模型评测”。
- Skill 执行主体与 1.0.2 比较，除新增“语言选择”章节外逐字一致；frontmatter 更新版本、语言与双语能力说明。其余执行、事实与授权规则保留。
- 文档中的 136 处 Markdown 相对链接目标存在，解析后均位于发布目录内，包括 docs/index.html；此项只检查目标文件，不验证远端页面、Release 下载或自动锚点。
- 全部文档、清单与 Skill 文本未检出邮箱、私有插件 ID、本机用户目录路径、常见 GitHub/API 令牌格式或私钥头。特定模式扫描不能保证发现所有敏感内容。
- 根目录与 Skill 目录的 LICENSE、NOTICE.md 与 1.0.2 字节一致。中文与英文独立 TXT 保留来源说明与完整 MIT License。

The document, manifest, and Skill checks cover 37 UTF-8 files, excluding the offline tool in `docs/`. JSON and YAML parse successfully; manifest identity, version, presentation, and subtitle length are consistent. Both plugin defaultPrompt values and the Skill agent default_prompt are preserved. The original 15 behavioral cases are unchanged, and the 3 added language cases bring the authored total to 18. The existing Skill execution body is unchanged apart from the added language-selection section. All 136 local Markdown links resolve inside the package. Targeted sensitive-text patterns found no matches. Root and Skill licenses and attribution notices are byte-identical to 1.0.2.

## 离线工具交互 / Offline tool interactions

实际浏览器检查结果见 [docs/VALIDATION.md](docs/VALIDATION.md)，涵盖界面语言切换、独立输出语言、输入保留、示例替换保护、复制、TXT 下载及窄屏排版。该检查与模型行为评测分开记录。

See the separate browser-check record for the offline tool. Interface checks and model behavior evaluations are distinct.

## 未执行与边界 / Not verified and limits

- 所有 18 个行为用例均未运行模型行为评测；未测成功率、准确率、效率或跨模型差异。语言规则的存在不证明模型在实际任务中总能遵守。
- 示例预期结构与参考片段是使用 AI 辅助编写的验收说明，不是已运行模型的输出或测试成绩。
- 本文档检查不证明离线工具的交互功能；浏览器交互与复制、下载的实际检查由离线工具的单独检查记录补充。
- 未执行宿主导入、账号安装、启用或长期使用验证；源码校验不能证明这些状态。
- 不审计公开仓库 Git 历史、缓存、其他副本或账号设置；不能据此声称历史邮箱已清除或安全漏洞已修复。
- 外部链接与 Release 下载必须在发布后另行核验；离线提示词工具不调用模型、不上传输入、无密钥，不等于外部 AI 产品对随后粘贴内容的处理保证。

No behavioral model evaluations have run. No success-rate, accuracy, efficiency, or cross-model improvement is established. Example outputs are authored acceptance guidance. These document checks do not prove browser interactions, host import, installation, account enablement, Git-history privacy, remote download availability, or external AI providers' data handling. Browser interaction checks are recorded separately for the offline tool.
