# Industry Analysis SOP

> 产业洞察SOP v1.0 — A systematic industry analysis framework based on Wang Yuquan's (王煜全) methodology from "学会洞察行业" (Mastering Industry Insights).

基于王煜全《学会洞察行业》方法学的系统性行业分析框架。经过4个跨行业案例验证，覆盖制造业、软件、前沿技术三类行业。

---

## Features / 特性

- **Three industry templates** / 三套行业模板：Manufacturing (制造业), Software (软件业), Frontier Technology (前沿技术)
- **Two analysis modes** / 两种模式：`--quick` (快速扫描, 4 steps) and `--full` (完整分析, 18 steps)
- **18-step SOP** / 18步标准流程：From industry boundary definition to scenario matrix and signal tracking
- **4 validated case studies** / 4个验证案例：CGM, AI Coding Tools, Solid-State Battery, Nuclear Fusion

## Installation / 安装

### Via GitHub (recommended / 推荐)

```bash
/plugin add hongjianz/industry-analysis
```

Then reload plugins:
```bash
/reload-plugins
```

### Usage / 使用

```bash
# Quick scan / 快速扫描
/skill:industry-analysis --quick <industry-name>

# Full analysis / 完整分析
/skill:industry-analysis --full <industry-name>

# Examples / 示例
/skill:industry-analysis --quick 固态电池
/skill:industry-analysis --full AI编程工具
```

### Modes / 模式说明

| Mode | Steps | Duration | Use Case |
|------|-------|----------|----------|
| `--quick` | 4 steps | 1-2 turns | Quick assessment / 快速判断 |
| `--full` | 18 steps | 3-5 turns | Deep analysis / 深度分析 |

## Structure / 目录结构

```
industry-analysis/
├── .claude-plugin/
│   └── marketplace.json          # Plugin manifest
├── industry-analysis/            # Plugin source
│   └── skills/
│       └── industry-analysis/
│           ├── SKILL.md          # Core instructions (入口指令)
│           ├── references/
│           │   ├── SOP-v1.0.md   # Full SOP reference (完整SOP参考)
│           │   ├── templates/    # Industry templates (行业模板)
│           │   └── examples/     # Case studies (案例精要)
│           ├── scripts/          # Helper scripts (辅助脚本)
│           └── assets/           # Templates (模板资源)
├── README.md
└── LICENSE
```

## Methodology / 方法学

This framework is based on Wang Yuquan's (王煜全) "Industrial Insights Methodology" (产业洞察方法学), which includes:

本框架基于王煜全的产业洞察方法学，核心包括：

- **Leading indicators vs lagging indicators** / 超前指标 vs 滞后指标
- **Supply/ecosystem chain scarcity analysis** / 产业链/生态链稀缺性分析
- **Four-step prediction method** / 四步预测法 (key variables → scenarios → signals)
- **Pyramid structure output** / 金字塔结构输出

## Case Studies / 验证案例

| Case | Industry Type | Key Insight |
|------|--------------|-------------|
| CGM | Manufacturing | Supply chain scarcity determines pricing power |
| AI Coding Tools | Software | Model capability + developer lock-in as moats |
| Solid-State Battery | Manufacturing Transition | Multi-route parallel + staged switching |
| Nuclear Fusion | Frontier Technology | "Shovel sellers" profit before miners |

## License / 许可证

[MIT](LICENSE)
