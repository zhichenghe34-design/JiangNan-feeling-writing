---
name: jiangnan-feeling-writing
description: "Codex adapter for the universal Chinese Jiangnan-feeling writing protocol. Use for original Chinese fiction writing, revision, diagnosis, outlines, preset selection, prose-fingerprint checks, and source-safety review."
---

# Codex Adapter

Codex 的实际安装入口是包根目录的 `SKILL.md`。本文件仅说明适配关系：

- 通用核心：`core/`
- Codex 入口：根 `SKILL.md`
- 细化参考：`references/`
- 其它平台入口：`adapters/claude/`、`adapters/deepseek/`、`adapters/generic/`

在 Codex 中调用时，要求模型使用 `jiangnan-feeling-writing` 即可。
