# 我是中国人 (I Am Chinese)

为 AI Agent 构建的中国文化角色扮演技能库。每个 skill 让 AI 能够准确理解和扮演中国不同地区/人群的角色。

## 项目简介

本项目为 AI Coding Agent 提供一组**中国文化技能 (skills)**，使其能够：

-   用地道的方言和文化特征与用户交流
-   准确理解不同地区人群的历史、习俗、价值观
-   在回答问题时采用对应地区的语言风格和思维方式
-   提供真实、尊重、全面的文化知识

**欢迎全国各地的开发者加入，一起打造属于中国人的 AI！**

### 参与方式

-   贡献你家乡地区的 skill
-   完善已有 skill 的内容
-   提出 AI 角色扮演的改进建议

## 当前收录

| 地区/人群 | 状态    | Skill 文件                      |
| --------- | ------- | ------------------------------- |
| 客家人    | ✅ 完成 | `.claude/skills/hakka/SKILL.md` |

## 项目结构

```
i-am-chinese/
├── .claude/
│   └── skills/              # Claude Code Skills 目录
│       └── hakka/           # 客家人
│           ├── SKILL.md     # Skill 入口文件
│           ├── validate.md  # Skill 验证测试
│           └── references/  # 详细参考文档
│               ├── architecture.md   # 建筑特色
│               ├── customs.md       # 风俗习惯
│               ├── events.md        # 历史大事
│               ├── food.md          # 美食文化
│               ├── geography.md     # 地理分布
│               ├── history.md       # 历史演变
│               ├── language.md      # 语言特点
│               └── people.md        # 历史人物
├── prompts/
│   └── validation.md        # Skill 验证提示词模板
└── README.md
```

## 如何使用

### 在 Claude Code 中使用

Claude Code 会自动发现 `.claude/skills/` 目录下的所有 skills。

**示例对话：**

```
User: "用客家人的口吻介绍你自己"
AI: "涯系客家人！涯嘅祖先系从中原南迁嘅汉人..."
```

```
User: "客家人有什么特色美食？"
AI: "讲到客家菜，涯兜人最骄傲嘅就系盐焗鸡啦..."
```

### 浏览学习

直接查看 `references/` 目录下的详细文档，深入了解：

-   客家土楼的建筑智慧
-   客家迁徙的历史脉络
-   客家方言的语言特色
-   客家名人的生平事迹

## Skill 结构规范

每个 skill 遵循统一的结构：

### SKILL.md (入口文件)

```yaml
---
name: skill_name
description: '简短描述 skill 的用途'
---
```

包含：

-   角色扮演指南
-   核心短语对照表
-   参考文档索引
-   使用示例

### references/ (参考文档)

| 文件            | 内容                     |
| --------------- | ------------------------ |
| architecture.md | 建筑特色（如土楼）       |
| customs.md      | 风俗习惯（如节日、礼仪） |
| events.md       | 历史大事（如迁徙事件）   |
| food.md         | 美食文化（如特色菜）     |
| geography.md    | 地理分布（如聚居地）     |
| history.md      | 历史演变（如迁徙史）     |
| language.md     | 语言特点（如方言特征）   |
| people.md       | 历史人物（如名人）       |

### validate.md (验证测试)

用于测试 skill 的正确性和完整性。

## 贡献指南

欢迎添加新的地区/人群 skill！

### 添加新 Skill

1. 在 `.claude/skills/` 下创建新目录
2. 创建 `SKILL.md` 入口文件
3. 创建 `validate.md` 验证文件
4. 在 `references/` 下添加参考文档
5. 参考现有 skill 的结构和风格

### 内容原则

-   **真实性**：确保内容符合该群体的真实文化特征
-   **尊重性**：避免刻板印象和歧视性内容
-   **全面性**：平衡地呈现文化特点
-   **实用性**：内容应能帮助 AI 准确理解和扮演该角色

### Pull Request

提交 PR 时请注明：

-   新增的地区/人群名称
-   主要内容概述
-   参考资料来源（如有）

## 待添加地区/人群

-   [ ] 广府人
-   [ ] 更多...

## 许可证

MIT License
