# 江南感写作 · jiangnan-feeling-writing

一套**平台无关**的中文原创写作协议,用于在原创小说里调出一种"江南式"的笔法运动与情感姿态:青春回望、缺口人物、远处的温暖、迟到的疼、信念付费、宏大与微物之间的转换。

版本:**v1.1.1**

## 这是什么

- 一个可被 Codex、Claude、DeepSeek 及通用 LLM 调用的写作 skill。
- 通用核心 `core/` + 平台适配 `adapters/` + 各平台入口的架构。
- 面向**原创写作、改稿、诊断、大纲**四类任务。

## 这不是什么

- **不是**同人或官方续写工具。
- **不是**复制任何源作品(人物、组织、设定、专名、桥段、源近句式)的工具。
- **不是**靠雨、天台、孤独、短句堆出来的表面仿写。

最终 skill 与最终生成文本都做到**零原文摘录(quote-free / source-excerpt-free)**。详见 [`references/safety-and-boundary.md`](references/safety-and-boundary.md)。

## 目录结构

```
SKILL.md                     Codex 可安装入口
core/                        平台无关协议(真正的核心)
  protocol.md                写作协议 + 选择成本规则
  presets.md                 阶段/配置 preset + 成本焦点
  fingerprints.md            页面级笔法指纹
  evaluation.md              评分门 + 失败模式
  install-and-use.md         安装与各平台调用
adapters/                    各平台入口提示
  codex/  claude/  deepseek/  generic/
agents/openai.yaml           OpenAI agent 配置
references/                  更细的内部参考(prose/preset/workflow/卡片/边界)
legacy_english_v1.0_*/       英文 v1.0 旧版,仅作对照存档
```

## 快速开始

按你的平台读对应入口:

- **Codex**:从 [`SKILL.md`](SKILL.md) 开始,按其调用流程读 `core/`。
- **Claude**:见 [`adapters/claude/CLAUDE.md`](adapters/claude/CLAUDE.md)。
- **DeepSeek**:把 [`adapters/deepseek/写作模式投喂提示.md`](adapters/deepseek/写作模式投喂提示.md) 复制进对话。
- **通用 LLM**:见 [`adapters/generic/system_prompt.md`](adapters/generic/system_prompt.md)。

核心调用顺序见 [`core/protocol.md`](core/protocol.md);交稿/测试前用 [`core/evaluation.md`](core/evaluation.md) 的 24 分评分门自检。

## v1.1.1 关键点

写作前必须确认**"现实成本 / 为什么他会选择"**:人物不只是被物件触动,还要在钱、身份、关系、工作、名誉、身体、机会或阵营上付出代价。成本必须通过物、动作、对话或制度细节露出来,**不用议论文解释**。

## 边界声明

这不是法律意见。对外发布或商业使用前请咨询专业知识产权律师。本仓库不含任何受版权保护的源作品原文或语料。
