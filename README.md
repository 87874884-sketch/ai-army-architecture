# 🛡️ AI Army Architecture / AI 军团架构

> 14 AI engines. 8 models. 4 brain layers. One person. / 14个AI引擎，8种模型，4层大脑，1个人。
> Self-evolving industrial manufacturing system. / 自学演化的工业制造系统。

[English](#english) | [中文](#中文)

---

## English

### The Army

```
🖥️ STRATEGIC BRAIN (Windows)
  WCC: DeepSeek V4 Pro          — Commander, coding, planning
  Zhao Yun: Doubao-Seed-2.0-Pro  — Deep analysis, cross-domain
  Gemma 4 12B (LM Studio)       — Local vision, CAD reading
  Agnes 2.0 Flash ×2            — Free cloud, text+image+video
  Cursor Composer 2.5            — Coding agent
  JuggernautXL (AI Playground)   — Local image generation

🔌 EXECUTION BRAIN (Jetson Xavier NX, 7×24)
  JCC: Claude Code + DeepSeek V4 Flash
  Ma Chao: Agnes API (free cloud scanning)

☁️ AUDIT BRAIN
  Huang Zhong (WCX): qwen3.6-plus + Agnes
  Mirror Brain: Cursor + WCX — Third-person system audit

📐 CAD PIPELINE
  Vision: 3-tier → CAD: CadQuery 2.7 → Nesting: PyNest → G-code: 16 posts
  Self-check: cad_validate.py + cad_selfcheck.py + 21 correction rules
```

### The Five Tigers — Recursive Knowledge Refinement

```
Ma Chao(scan) → Zhao Yun(analyze) → Internet Validation →
Zhang Fei(challenge) → Guan Yu(rule) → Huang Zhong(audit) →
Code Fix → Regression Test → ↻ Loop
```

**Key innovation:** Internet validation as objective anchor. Every AI claim must survive real-world data before becoming code. This breaks the "AI hallucination cascade" — no model can bullshit its way past a WebSearch.

**Results:**
- Round 1: 10 insights → 15 proposals → 13 issues found → 9 fixed
- Round 2: Systemic "cognition-execution gap" autonomously discovered
- Round 3+: Fully automated, no human needed

### Hardware

| Device | Spec | Max Model |
|--------|------|-----------|
| Windows | Intel Arc 140T 16GB / 32GB RAM | ~12B @ Q4 |
| Jetson NX | 6.7GB RAM, ARM64 | ~3B @ Q4 |
| Cloud Free | Agnes 44RPM + Doubao 50万 tokens | — |

### Key Metrics

| Metric | Value |
|--------|-------|
| Python scripts | 22 |
| Regression tests | 7 parts, 6/6 passing |
| Validation records | 34 (23✅ 6⚠️ 5❌) |
| CAD correction rules | 21 rules |
| CAD vision accuracy | 97% (multi-pass CV+12B) |
| Pipeline status | extract(12B) → deepen → WCX(auto) → code |

### Philosophy

- **Every bug = a missing process step.** Install a guardrail, don't blame the model.
- **Recursive self-improvement.** The system audits the system that builds the system.
- **Free front, paid back.** Free models scan; paid models rule.
- **One person + 14 AI = manufacturing plant.** 3,800-unit order, processed autonomously.
- **Essays:** [docs/essays/](docs/essays/) — *The Meaning of AI* (EN+ZH), complement to Pageau @ ARC 2026 (2026-07-05)

---

## 中文

### AI 军团阵容

```
🖥️ 战略脑 (Windows)
  关羽 WCC: DeepSeek V4 Pro         — 总指挥、编码、规划
  赵云: 豆包 Doubao-Seed-2.0-Pro    — 深度分析、跨域关联
  本地: Gemma 4 12B (LM Studio)     — 视觉识图
  免费云端: Agnes 2.0 Flash ×2     — 文本+图片+视频
  Cursor Composer 2.5               — 编码助手
  AI Playground JuggernautXL        — 本地生图

🔌 执行脑 (Jetson Xavier NX, 7×24小时)
  JCC: Claude Code + DeepSeek V4 Flash
  马超 JXQ: Agnes API (免费云端扫描)

☁️ 审查脑
  黄忠 WCX: qwen3.6-plus + Agnes — 代码审查、合规验证
  镜子脑: Cursor + WCX — 第三方视角照见系统问题
```

### 五虎知识精炼闭环

```
马超(扫描) → 赵云(分析) → 全网验证 → 张飞(挑战) → 关羽(裁决) → 黄忠(审计) → 代码修复 → 回归测试 → ↻ 循环
```

**核心创新：** 第4步"全网验证"打破了AI自嗨循环。每种说法必须经过真实互联网数据检验，才能进入代码层。验证通过✅、修正⚠️、推翻❌——这个标记机制斩断了模型间的"幻觉滚雪球"。

**实测数据：**
- 第一轮：10条感悟 → 15个提案 → WCX发现13个问题 → 修了9个
- 第二轮：系统自主发现"认知-执行断层"
- 第三轮起：全自动，不需要人工提醒

### 硬件架构

| 设备 | 配置 | 最大模型 |
|------|------|---------|
| Windows | Arc 140T 16GB显存 / 32GB内存 | ~12B Q4量化 |
| Jetson NX | 6.7GB内存, ARM64 | ~3B Q4量化 |
| 免费云端 | Agnes 44次/分钟 + 豆包50万tokens | — |

### 关键指标

| 指标 | 数值 |
|------|------|
| Python 脚本 | 22 个 |
| 回归测试 | 7 个零件, 6/6 通过 |
| 代码追溯 | 34 条 (23✅ 6⚠️ 5❌) |
| CAD 修正规则 | 21 条 |
| CAD 识图精度 | 97% (CV多遍法+12B) |

### 核心理念

- **每个Bug = 流程缺一个步骤。** 不责备模型，装永久护栏。
- **递归自我改进。** 审查系统的系统，构建系统的系统。
- **前端免费，后端付费。** 免费模型做扫描，付费模型做裁决。
- **一个人 + 14个AI = 制造工厂。** 3800件订单已全自动处理。
- **随笔：** [docs/essays/](docs/essays/) — 《AI 时代的意义》（中+EN），与 Pageau @ ARC 2026 互补（2026-07-05）

---

### The Author / 作者

Solo developer in Harbin, China. Not VC-backed. Not a startup. One person, 14 AI engines, one vision: fully automated sheet metal manufacturing.

中国哈尔滨，独立开发者。没有风投，不是创业公司。一个人，14个AI引擎，一个愿景：全自动钣金制造。

*Built with: Claude Code (DeepSeek V4 Pro), Cursor Composer 2.5, Gemma 4 12B, Agnes AI, Doubao-Seed-2.0-Pro, qwen3.6-plus, CadQuery, PyNest, OpenCV, ComfyUI*
