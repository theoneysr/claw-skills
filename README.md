# OpenClaw Skills 仓库

各种 OpenClaw AI 代理使用的技能包集合。

## 📖 什么是 Skills？

Skills 是 OpenClaw AI 代理的可扩展模块，为代理提供特定的能力和功能。每个技能都是一个自包含的模块，包含：

- **SKILL.md** - 技能描述和使用说明
- **脚本文件** - 实现技能功能的脚本
- **配置文件** - 技能所需的配置
- **文档** - 原著依据或技术文档

## 🚀 如何使用

### 1. 安装 Skill

将技能目录复制到 OpenClaw 的扩展目录：

```bash
# 克隆这个仓库
git clone https://github.com/theoneysr/claw-skills.git

# 复制你需要的技能到 OpenClaw 扩展目录
cp -r claw-skills/skills/your-skill ~/.openclaw/extensions/
```

### 2. 重启 OpenClaw

安装技能后，需要重启 OpenClaw Gateway：

```bash
openclaw gateway restart
```

### 3. 使用 Skill

在对话中，OpenClaw 会自动检测可用的技能并根据对话内容选择合适的技能。

## 📚 现有 Skills

### 🔴 求是 Skill 包

基于教员思想提炼的方法论工具集，系统性武装 AI 的大脑。

**10 个核心技能：**

1. **arming-thought** - 武装思想
   - 建立实事求是总原则
   - 任务路由框架
   - [查看详情](skills/arming-thought/SKILL.md)

2. **contradiction-analysis** - 矛盾分析法
   - 识别矛盾、抓住主要矛盾
   - 复杂问题分析
   - [查看详情](skills/contradiction-analysis/SKILL.md)

3. **practice-cognition** - 实践认识论
   - 实践→认识→再实践
   - 方案验证与迭代
   - [查看详情](skills/practice-cognition/SKILL.md)

4. **investigation-first** - 调查研究
   - 没有调查就没有发言权
   - 决策前的信息收集
   - [查看详情](skills/investigation-first/SKILL.md)

5. **mass-line** - 群众路线
   - 从群众中来到群众中去
   - 反馈整合与方案验证
   - [查看详情](skills/mass-line/SKILL.md)

6. **criticism-self-criticism** - 批评与自我批评
   - 惩前毖后，治病救人
   - 工作审视与质量改进
   - [查看详情](skills/criticism-self-criticism/SKILL.md)

7. **protracted-strategy** - 持久战略
   - 战略上藐视，战术上重视
   - 长期复杂任务规划
   - [查看详情](skills/protracted-strategy/SKILL.md)

8. **concentrate-forces** - 集中兵力
   - 集中优势兵力各个歼灭
   - 优先级决策与资源聚焦
   - [查看详情](skills/concentrate-forces/SKILL.md)

9. **spark-prairie-fire** - 星火燎原
   - 建立根据地，不做流寇
   - 从零开始的发展策略
   - [查看详情](skills/spark-prairie-fire/SKILL.md)

10. **overall-planning** - 统筹兼顾
    - 调动一切积极因素
    - 多目标平衡与权衡
    - [查看详情](skills/overall-planning/SKILL.md)

**更多详情：** [求是 Skill 官方文档](https://github.com/HughYau/qiushi-skill)

### 其他 Skills

查看 [skills/](skills/) 目录了解所有可用的技能。

## 🤝 贡献

欢迎贡献新的技能！

### 提交 Skill 的步骤：

1. Fork 这个仓库
2. 创建你的技能目录
3. 按照 [技能模板](SKILL_TEMPLATE.md) 创建你的技能
4. 提交 Pull Request

### Skill 模板

每个技能应该包含：

```
your-skill/
├── SKILL.md              # 必需：技能描述
├── scripts/              # 可选：脚本文件
│   └── your-script.js
├── config/               # 可选：配置文件
│   └── config.json
└── docs/                 # 可选：文档
    └── original-texts.md
```

## 📝 许可证

求是 Skill 包采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件。

## 🔗 相关链接

- [OpenClaw 官方文档](https://docs.openclaw.ai)
- [OpenClaw GitHub](https://github.com/openclaw/openclaw)
- [ClawHub](https://clawhub.com) - OpenClaw 技能市场

## 📧 联系

- 作者: theoneysr
- GitHub: [@theoneysr](https://github.com/theoneysr)

---

**让 OpenClaw 更强大，一个技能一个技能！** 🚀
