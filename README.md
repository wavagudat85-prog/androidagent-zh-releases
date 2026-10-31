# AndroidAgent 简体中文社区版

这是基于 [mateuszsury/androidagent v0.5.0](https://github.com/mateuszsury/androidagent/tree/v0.5.0) 的独立社区版发布仓库，不是 OpenAI、Anthropic 或原作者的官方中文版本。

[下载安装包、源码和校验文件](https://github.com/wavagudat85-prog/androidagent-zh-releases/releases/latest)

本次助理分支新增：

- 默认数字助理入口。选择 AndroidAgent 后，系统支持的助理手势可以打开当前对话。小米还需在系统中配置电源键手势；部分国行 HyperOS 固件固定调用小爱，实际支持情况需在手机上验证。
- 应用内 GitHub 更新。设置 → 唤醒与更新 → 应用更新，优先下载与本机版本和 APK 摘要完全匹配的 HDiffPatch 补丁，失败回退完整 APK，校验后交由 Android 安装器确认。

首次从 zh.2 升级，需安装一次完整 APK，之后才有应用内更新入口。`.hdiff` 是差分文件，不能直接点击安装。首次安装及没有匹配补丁时，请下载 `.apk`。

本分支保留 zh.2 的原有对话逻辑；原对话中的 Codex 问答问题由另一开发分支继续处理。相同应用 ID 与社区签名允许覆盖更新，保留原有数据。

每次发布包含完整 APK、适用的增量补丁、`update.json`、`SHA256SUMS.txt` 和对应源码 ZIP。源码包保留上游及第三方许可、构建和验证工具；HDiffPatch 使用 MIT 许可，运行时组件各自适用其原有许可。
