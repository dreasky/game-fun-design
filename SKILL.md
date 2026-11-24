---
name: game-fun-design
version: "0.1.0"
display_name: 游戏快乐设计
display_name_en: Game Fun Design
description: 用《游戏设计快乐之道》(A Theory of Fun for Game Design, Raph Koster) 的乐趣模型来诊断玩法为什么不好玩、反向推导新玩法点子、查阅书中概念与术语。当讨论"这个机制有没有意思""玩家为什么会腻""核心循环""学习曲线/难度节奏""关卡或系统设计是否成立"时使用。Also use when discussing whether game mechanics are fun, player boredom, core loop design, or learning curves.
description_zh: 用《游戏设计快乐之道》的乐趣模型诊断玩法为什么不好玩、倒推新玩法点子、查阅概念与术语。当讨论"这个机制有没有意思""玩家为什么会腻""核心循环""学习曲线/难度节奏""关卡或系统设计是否成立"时使用。
description_en: Use the fun model from A Theory of Fun for Game Design to diagnose why gameplay is not fun, reverse-engineer new mechanics, and look up concepts and terms. Use when discussing whether game mechanics are fun, player boredom, core loops, learning curves, difficulty pacing, or whether a level or system design holds up.
---

# 游戏快乐设计

把"好不好玩"从直觉变成可操作的分析。核心立场：**快乐分门类，每类有各自的供给机制与失效方式**——"不好玩"不是一种病，先归因、再上轴、最后给旋钮。

## 先三问（任何分析的第一步）

| # | 问什么 | 决定什么 | 详见 |
|---|---|---|---|
| 1 | **归因**：在供给哪种快乐？ | 门类不同，同一症状的解法方向相反 | `references/core-model.md` §1 |
| 2 | **表达**：想传递什么情感体验？ | 轴给的是快乐最优位，不是应该在的位置；痛苦可能是表达载体 | `core-model.md` §2.1 |
| 3 | **目标**：教完还是长寿？ | 教完模型里玩家学完走人是完成；长寿模型里才是失败 | `core-model.md` §2.2 |

归到学习快乐后，再问：**玩家此刻在学什么模式？他离掌握它还有多远？**

本知识库守 Koster 的**窄定义**：`fun` 专指学习型快乐（识别→内化→自动化的整段过程）。秩序、张力、身体各立门类；审美/叙事/社交是表达层载体 `[存疑]`，不混称"乐趣"。

## 文件地图

| 文件 | 内容 | 何时读 |
|---|---|---|
| `references/core-model.md` | 快乐门类、表达、学习循环、保质期、探索、秩序、张力、迁移 | 需要模型/判据 |
| `references/diagnose.md` | 症状速查表 + 14 条轴（含平衡手册）+ 常见误诊 | 模式 A 诊断 |
| `references/variable-sources.md` | 变量源、寿命、破圈、透明测试 | 模式 C 判寿命 |
| `references/ideate.md` | 从"要教什么"倒推机制的六步 | 模式 B 生成 |
| `references/glossary.md` | 术语表 | 查词 |
| `notes/00-index.md` | 建设日志：确立/推翻/欠账 | 查建设状态 |

## 四种工作模式

| 模式 | 做什么 | 输出 |
|---|---|---|
| **A 诊断** | 先三问 → 描模式结构（核心动词/变量/反馈）→ 用该门类双端失效轴定位 | 症状/定位/动作三段；动作落到"改哪个规则、加哪个变量、删哪个环节" |
| **B 生成** | 从"想让玩家学会什么"倒推机制（`ideate.md`）；缺素材翻 `variable-sources.md` §3 | 六步推导链 |
| **C 判寿命** | 数这个设计有几个不可穷尽的变量源（`variable-sources.md`） | 零个 → 只能靠做内容续命；有 → 说清深度与代价 |
| **D 查阅** | 按文件地图查模型/术语 | 直接答；`[存疑]` 要说清它悬着 |

**硬规则**：不许给"增加变化""让它更有趣"这类无法执行的建议。

不适用：性能优化、引擎实现、美术风格。商业化数值只在被当作"快乐的替代品"时进入讨论（透明测试，`variable-sources.md` §7）。

## 标记

本知识库是一套设计理论，不是某本书的摘要——条目不标出处，只标**这条站没站稳**。

| 标记 | 含义 | 用法 |
|---|---|---|
| `[存疑]` | 推理链有缺口、只有单个案例支撑、或与别处矛盾 | 可用来分析，但引用时必须说明它悬着；不得当成已确立的结论断言 |

没标记 = 可以直接用。一条规则若在不同情况下结论不同，那是内容（两种适用范围并列写出），不是标记。

**当前状态**：条目由讨论积累而成，未经书中原文逐条校订；引用时只说"按这套模型看"，不要把结论归给作者或这本书。

## 输出风格

- 先给判断，再给依据，最后给动作；不复述用户描述。
- 术语用原词（grok、噪音、模式），紧跟一句人话解释。
- 诊断输出控制在一屏；长清单放进文件，不在对话里铺开。
