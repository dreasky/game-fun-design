# game-fun-design

游戏快乐设计 skill。引擎无关，纯设计层。

以《游戏设计快乐之道》(Raph Koster, *A Theory of Fun for Game Design*) 为**起点**，但不是它的摘要——书中论断、现代案例（蔚蓝、黑魂、塔科夫、模拟器类）与实践判断共同支撑结论，冲突处两边并列、用适用范围区分。条目不标出处，只标 `[存疑]`（这条站没站稳）。

## 用途

- **诊断**：描述一个玩法/关卡/系统，得到"为什么不好玩"的结构化判断和可执行的修改动作
- **生成**：从"想让玩家学会什么"倒推出机制方案
- **判寿命**：估这个设计能撑多久，以及怎么把它拉长
- **查阅**：模型、判据、术语、建设日志

## 目录

```
game-fun-design/
├─ SKILL.md                  入口：三问、文件地图、四种模式、标记
├─ references/
│  ├─ core-model.md          核心模型（快乐门类、表达约束、学习循环、保质期）
│  ├─ variable-sources.md    变量源与寿命（素材库、深浅判据、破圈、透明测试）
│  ├─ diagnose.md            诊断流程 + 14 条轴（含平衡手册）
│  ├─ ideate.md              倒推法生成玩法
│  └─ glossary.md            术语表
└─ notes/
   └─ 00-index.md            建设日志：确立了什么、推翻了什么、还欠什么
```

编写过程的规则（先讨论后沉淀、可信度标记制度、归纳规范）在上级目录的 `../CLAUDE.md`，对本目录下所有 skill 通用。

## 安装

复制或链接到 skills 目录：

```powershell
# 用户级（所有项目可用）
Copy-Item -Recurse "D:\Project\Project_Godot\skill\game-fun-design" "$env:USERPROFILE\.claude\skills\"

# 或建符号链接，改动即时生效（需管理员权限）
New-Item -ItemType SymbolicLink -Path "$env:USERPROFILE\.claude\skills\game-fun-design" -Target "D:\Project\Project_Godot\skill\game-fun-design"
```

## 建设状态

正在随读书与讨论增量填充。条目由讨论积累而成，未经书中原文逐条校订——框架可用，但引用时只说"按这套模型看"，不要把结论归给作者。标记只有 `[存疑]`（这条站没站稳），没标记 = 可以直接用。

2026-11-13 按高注意力机制做了一次整改：`SKILL.md` 加文件地图与模式表，`core-model.md` 加"一页总览"，`diagnose.md` 加"轴速查"，全部判据与存疑清单保留。

存疑清单分布在 `core-model.md`（12 条）、`variable-sources.md`（5 条）、`ideate.md`（3 条），汇总视图见 `notes/00-index.md` 的"还欠什么"。
