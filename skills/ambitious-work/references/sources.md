# 来源、全文主题覆盖与归因

## 使用边界

本包把文章方法转成工作流程，不复制或提供原文全文、完整翻译、原图或外链作品。初版以项目早期整理的中文精读 PDF 和提示词为主要底稿，再用作者网页核对主题；公开版不分发该 PDF。正文中的详细执行协议、权限控制、测试用例与应用配方为本 Skill 新写。

“覆盖”表示相关主题有对应的操作规则或背景索引，不表示逐句收录；背景轶事不转换成证明任务可行的证据。原文内容仍应通过作者网站阅读。

## 主来源

**Felix Rieseberg — How to be more ambitious: A tutorial for humans with models**

网页标示发表日期：2026-10-13。核对日期：2026-10-21。

https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/

本文非官方 Skill，不暗示作者或 Anthropic 认可本实现。不因作者从事某项工作，就把他的经验判断提升成普遍结论。

## 对话内底稿

- 中文精读 PDF：初版使用的 8 页整理底稿，不是全文翻译；公开版已移除，执行本 Skill 不依赖该文件。
- [已有提示词](../assets/prior-prompts.md)：此前生成的 Markdown，原样附入；其提示词是整理者新写，不是原文原句。
- [本版提示词](../assets/prompts.md)：本次为可调用 Skill 增补的任务入口。

底稿覆盖了四种方向、季度复盘和客户流失示例、边界条件及作品集等应用场景。其来源标签应继续保留，不能把后加示例算到原作者名下。

## 全文主题对照

下表是定位索引。左栏为主题标签，右栏说明本 Skill 的处理位置，不重述原文论证。

| 原文位置 / 主题 | Skill 中的对应位置 | 处理方式 |
| --- | --- | --- |
| 开篇：能力不均与使用方式 | SKILL.md：任务选择、尝试与验证 | 不预设全能或无能 |
| 开篇：四种 ambition | SKILL.md：S / A / D / R | 方法路由 |
| Speed | playbook.md：效率操作 | 原文未展开；步骤为新增 |
| Altitude：目标与任务 | SKILL.md：高度 | 保留用户约束 |
| Altitude：季度复盘 | 作者网页的 Altitude 部分 | 保留阅读入口；公开版不附精读 PDF |
| Altitude：替代流程 | playbook.md：工具、环境与持续流程 | 新编执行协议 |
| Altitude：软件崩溃案例 | playbook.md：环境与权限 | 案例定位；不复述细节 |
| Altitude：创作适用性 | SKILL.md：何时使用 | 保留适用边界 |
| Depth：专业方法 | playbook.md：专业方法的选择 | 方法必须实际执行 |
| Depth：挑战目标 | playbook.md：实验约定 | 区分目标与证明 |
| Depth：检验假设 | playbook.md：反向检查 | 支持、反例与替代解释 |
| Depth：新发现 | playbook.md：新发现与验证分开 | 探索不等于验证 |
| Depth：独立评判 | playbook.md：外部检验 | 不以自评分验收 |
| Depth：四问提示词 | SKILL.md：深度开头 | 独立改写为工作问题 |
| Range：动词化 | SKILL.md：广度 | 以动作寻找方法 |
| Range：组合专业 | playbook.md：跨领域工作单 | 不模拟专家表演 |
| Range：多代理 | SKILL.md：工具真实性 | 仅在真实可用时委派 |
| Range：Blender / 主页 | 本页：案例背景索引 | 不转成用户经历 |
| 工具、软件与数据前提 | playbook.md：工具、环境与持续流程 | 授权和可用性检查 |
| We have been here before | SKILL.md：可承受的实验 | 动机转为可测试行动 |
| 自我效能与目标设定 | playbook.md：实验失败后的处理 | 不是效果保证 |
| 相信可试、观察示范、容许失败 | SKILL.md：第三步 | 不代替事实检验 |
| 结语 | SKILL.md：验收与迭代 | 依据观测调整 |
| 插图与作者简介 | 本页：背景索引 | 署名定位，不打包原图 |

## 案例与动机背景索引

作者还以科学、影像和数学进展说明能力变化，并援引自我效能、目标设定及人物故事谈尝试的心理门槛。这里保留索引，不把报道、经验或轶事当作本 Skill 的效果证据。

原文可对照的名称：Acme、Claude 崩溃修复、Alex Albert / Blender、Michelangelo、Locke & Latham、Patrick Collison、George Dantzig、Roger Bannister、Sabastian Sawe、The Inner Game of Tennis、Linux。历史年份、运动成绩或因果解释如需对外引用，应另查第一手来源；本包不据此作新的事实保证。

插图署名索引：Francisco Goya，Modo de volar。原图未收入。

## 进一步阅读入口

以下是原文或底稿列出的入口；保留链接不表示本次已经复核其中每一个研究结论。

- Locke & Latham，目标设定研究：
  https://med.stanford.edu/content/dam/sm/s-spire/documents/PD.locke-and-latham-retrospective_Paper.pdf
- Patrick Collison，Fast：
  https://patrickcollison.com/fast

外部论文未重新打包；实际使用其中的结论时读取并核查适用条件，不直接从二手概述推出个人效果。

## 格式参考

- Agent Skills 格式：https://agentskills.io/specification
- OpenAI Skills：https://developers.openai.com/plugins/build/skills
- OpenAI Plugin 打包：https://developers.openai.com/plugins/build/plugins

这些来源只用于文件结构与插件封装，不为本工作法的效果背书。

## 公开分发与许可

本包的独立实现采用 MIT 许可证，见技能目录内的 LICENSE。第三方权利与归因边界见同目录 NOTICE.md；作者的文章、插图和外链论文不属于本项目的 MIT 授权范围。
