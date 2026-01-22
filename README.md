# 🛡️ LogSentinel

> **让 AI 成为你的 7x24 小时运维专家。**
> *Turn your logs into actionable insights with LLM Agents.*

## 📖 项目简介 (Introduction)

本项目是一个基于 **Java** 生态构建的 **AIOps 智能体 (Agent)**。
传统的日志监控只能做到“基于规则的报警”（如：错误数 > 10 则报警），而本 Agent 旨在利用 **大语言模型 (LLM)** 的推理能力，实现对 Nginx、Java 应用日志的**语义理解**、**故障归因**以及**自动修复建议**。

这是从传统 DevOps 向 **Agentic Workflow** 转型的一次实践。

## 🏗️ 技术架构 (Tech Stack)

* **核心语言**: Java 21
* **开发框架**: Spring Boot 4.x
* **AI 框架**: Spring AI / LangChain4j (计划兼容 DeepSeek, Qwen, OpenAI API)
* **基础设施**: Docker & Nginx (日志源)
* **数据处理**: Log Parsing & Deduplication (日志清洗与去重算法)

## ✨ 核心功能 (Features)

- [x] **智能日志清洗**: 自动识别并合并重复的异常堆栈，减少 Token 消耗。
- [ ] **多维分类诊断**: 自动将日志归类为 `配置错误`、`代码缺陷`、`恶意攻击`、`网络波动`。
- [ ] **人话日报**: 每天定时生成 Markdown 格式的运维日报，由 AI 总结当日健康度。
- [ ] **主动防御 (规划中)**: 针对恶意扫描日志，自动生成 Nginx Deny 规则或防火墙策略。

## 🗺️ 2026 演进路线图 (Roadmap)

1.  **Phase 1 (MVP)**: 实现读取 Docker 挂载的 Nginx 日志，调用 LLM API 生成简报。
2.  **Phase 2 (Automation)**: 接入 IM 机器人（钉钉/企微/飞书），实现实时告警。
3.  **Phase 3 (Agentic)**: 引入“工具调用 (Tool Use)”，赋予 Agent 执行命令的权限（如重启服务、封禁IP）。

## 🚀 快速开始 (Quick Start)

*(此处预留给未来写启动步骤)*
