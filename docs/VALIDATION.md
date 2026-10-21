# 双语工具交互检查 / Bilingual tool interaction checks

版本 / Version：1.1.0。检查日期 / Checked：2026-10-21。

以下项目已在真实浏览器中操作，不是模型行为评测：

- 中文与 English 界面切换后，四个输入字段保持不变。
- 输出语言可选中文、English 和中英双语；切换界面不改变已选输出语言。
- 英文入口 `?lang=en` 首次打开时，界面与初始输出语言均为 English。
- 英文模式生成英文执行要求，同时保留输入材料原文和数字。双语模式明确要求中英逐段对应、事实和引用一致。
- 点击复制后出现成功反馈；TXT 下载成功，包含中文与英文。
- 已有输入时点击示例会显示替换提示；取消后保留原输入，确认后载入明确标注的虚构教学材料。
- 390 像素宽度下，中文与 English 界面均未出现横向溢出。
- JavaScript 语法检查通过。源码无 fetch、XMLHttpRequest、WebSocket 或外部脚本、字体依赖；表单不上传输入，也不持久化输入。

Browser checks covered interface switching, independent output selection, the English entry, preserved input, paired bilingual instructions, clipboard feedback, TXT download, example replacement protection, and layout at a 390-pixel width. JavaScript syntax validation passed. The source has no network calls or external runtime dependencies, and does not persist form input.

本工具只构造提示词，不调用 AI。上述检查不证明外部模型会按提示词生成正确内容；18 个模型行为用例仍未运行。已验证的浏览器行为也不保证每种浏览器、系统剪贴板策略或宿主安装状态。

This tool builds prompts; it does not call a model. These checks do not establish output quality or guarantee behavior in every browser or clipboard policy. All 18 model behavior cases remain unexecuted, and host installation is outside this check.
