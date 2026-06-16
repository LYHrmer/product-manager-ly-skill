# product-manager-ly

一个**工具中立、自包含**的产品经理技能。它编码的是**前 0.1% 产品经理的思维纪律**——先界定问题再谈方案、证据优于意见、结果优于产出、残酷优先级与显式不做、交付前自我红队——而**不是又一套 PRD 填空模板**。

> 平庸 PM 发模板,所以产出千篇一律;顶尖 PM 走纪律。这个技能让 AI 每次都强制走纪律。

## 它做什么

- 把"想法/需求"逼着走完 6 道质量门:界定问题 → 证据 → 结果与指标 → 残酷优先级 → 写作 → 自我红队。
- 覆盖 PM 全流程的耐久能力:问题界定、用户探索、证据推理、战略定位、优先级、路线图、指标/OKR、PRD、上线决策、干系人对齐、自我评审。
- 内置**防捏造铁律**(绝不编造证据/数据/用户原话)和**每种产物的验收 rubric**。

## 它不做什么

- 不出原型、不写工程实施代码计划——产出 PRD 即交付,后续交给设计/工程。
- **不依赖任何其他技能**:别人裸装即可用。

## 安装

Claude 与 Codex 通用,装到哪个取决于你装了哪个工具。

```bash
git clone <this-repo> product-manager-ly
cd product-manager-ly
./scripts/install.sh          # 默认拷贝;探测 ~/.claude/skills 与 ~/.codex/skills
./scripts/install.sh --dev    # 开发模式:软链接,改源仓库两边即时生效
```

Windows:

```powershell
.\install.ps1
```

幂等:重复运行覆盖更新。改内容请编辑本源仓库再重新 install。

## 卸载

```bash
rm -rf ~/.claude/skills/product-manager-ly ~/.codex/skills/product-manager-ly
```

## 结构

- `SKILL.md` — 核心论点 + 6 步纪律主线 + 危险信号 + reference 地图(短,按需展开)。
- `references/` — 11 篇深度纪律(各自开头先给最锋利的一条)。
- `templates/` — 8 个产物模板,每个带"反模板"护栏(模板是思考脚手架,不是填空表)。
- `references/example-walkthrough.md` — 一个端到端走查示例,每步好/坏对照。
