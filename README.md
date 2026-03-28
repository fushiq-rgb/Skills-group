# 013-prd-agent

PRD需求工作流技能。从原始需求素材出发，经4个独立Agent角色（会议转录整理→业务意图翻译→PRD结构化写作→评审挑战模拟）协作产出完整PRD文档。

## 技能结构

```
013-prd-agent/
├── SKILL.md                       # 技能主入口
└── references/
    ├── 01-recorder.md             # Agent1：会议转录与事实整理员
    ├── 02-intent-translator.md    # Agent2：业务意图翻译官
    ├── 03-prd-writer.md           # Agent3：PRD结构化写手
    └── 04-reviewer.md             # Agent4：评审挑战模拟器
```

## 触发词

"开始PRD流程"、"整理需求"、"写PRD"、"做需求评审"、"启动PRD流水线"

## 工作流

1. **Agent1（Recorder）**：读取原始素材，输出共识事实/猜测/待决事项清单
2. **Agent2（Intent Translator）**：将业务诉求翻译为可量化目标+约束清单
3. **Agent3（PRD Writer）**：输出标准PRD初稿，六大核心模块完整
4. **Agent4（Reviewer）**：多角色评审挑战，输出风险分级+工单草案

## 质量原则

- **零推测**：每个输出项必须有明确来源依据
- **零跨区**：各Agent严格遵守分区边界，不读取非必要分区内容
- **脱敏前置**：敏感信息写入文档前必须完成占位符替换
- **完成确认规范化**：每个Agent输出末尾必须包含标准化完成声明

## 飞书文档协作

全流程共用1份飞书文档，5个分区隔离（原始素材区→Agent1→Agent2→Agent3→Agent4）。
