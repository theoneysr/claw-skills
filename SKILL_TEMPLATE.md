# Skill 模板

复制此模板来创建新的 Skill。

## 目录结构

```
your-skill/
├── SKILL.md              # 必需：技能描述（就是这个文件）
├── scripts/              # 可选：脚本文件
│   └── your-script.js
├── config/               # 可选：配置文件
│   └── config.json
└── docs/                 # 可选：文档
    └── original-texts.md
```

## SKILL.md 格式

SKILL.md 是技能的核心描述文件，包含以下内容：

```markdown
---
name: your-skill
description: |
  技能触发条件的描述。在什么情况下会激活这个技能？
  English: Description of when this skill should activate.
---

# [技能名称]

## 技能描述

详细描述这个技能的功能和用途。

## 使用场景

在什么情况下会激活这个技能？

## 功能特性

列出这个技能提供的主要功能。

## 使用方法

详细说明如何使用这个技能。

## 配置说明

如果需要配置，说明配置项的含义。

## 技术实现

简要说明技术实现细节。

## 注意事项

使用时需要注意的事项。
```

## 示例 Skill

参见 [skills/](skills/) 目录中的示例技能。

## 技能规范

1. **SKILL.md 必须存在** - 这是技能的核心描述文件
2. **相对路径处理** - 如果技能文件引用相对路径，确保相对于技能目录解析
3. **工具使用** - 技能可以使用 OpenClaw 提供的工具
4. **独立性** - 每个技能应该是独立的，不依赖其他技能

## 开发指南

### 激活条件

技能的激活条件在 SKILL.md 的 description 中定义。OpenClaw 会根据对话内容自动选择合适的技能。

### 工具访问

技能可以通过以下方式访问工具：
- 读取工具文档：`/usr/lib/node_modules/openclaw/tools/TOOL_NAME.md`
- 使用技能特定的脚本文件

### 测试

测试你的技能：
1. 安装技能到 OpenClaw 扩展目录
2. 重启 OpenClaw Gateway
3. 在对话中测试技能的激活和行为

## 提交指南

1. 确保技能目录结构完整
2. SKILL.md 包含完整的技能描述
3. 测试技能可以正常工作
4. 提交 Pull Request
