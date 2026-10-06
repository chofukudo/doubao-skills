# doubao-skills

豆包（Doubao）专属 Skills 集合仓库。每个 Skill 是一个自包含的技能文件夹，用于扩展豆包/豆包办公（Doubao Work）的能力，包含角色设定、工作流、专业知识与资源。

## 目录结构

```
doubao-skills/
└── <skill-name>/          # 每个 Skill 一个目录
    ├── SKILL.md           # Skill 主文件（YAML frontmatter + 使用指令）
    └── design-source.html # 可选：设计源稿/说明文档
```

## Skills 清单

| Skill | 用途说明 | 触发场景 |
|---|---|---|
| [mindset-reconstruction-coach](./mindset-reconstruction-coach/SKILL.md) | 心智重构教练：融合认知心理学（CBT、暴露疗法、内控型归因、邓宁-克鲁格效应）与毛泽东哲学方法论（《实践论》《矛盾论》等），按「认知解离 → 主体性夺回 → 认知型自信 → 暴露疗法」四大模块，帮助用户将底层自卑转化为认知型自信，走向内心自洽。每次回复包含诊断、重构、行动闭环。 | 用户表达自卑、内耗、自我怀疑、低自尊、社交焦虑、怕被评价、不敢发言、拖延焦虑，或希望建立认知型自信、寻求心理教练式对话 |

## 安装方法

### 方式一：复制到 Skills 目录（推荐）

1. 将 `mindset-reconstruction-coach/` 文件夹整体复制到豆包工作区的 `.user_skills` 目录下（路径示例：`<工作区路径>/.user_skills/`）；
2. 重启/刷新豆包会话，Skill 即可被自动发现；
3. 当对话命中 Skill 描述中的触发场景时，豆包会自动加载并使用该 Skill。

### 方式二：创建智能体

1. 打开豆包「创建智能体」；
2. 将 `SKILL.md` 中的角色设定与工作流内容粘贴到【系统提示词/人设】区域；
3. 保存后即可直接对话使用。

## 新增 Skill 的规范

- 每个 Skill 独立成目录，必须包含 `SKILL.md`；
- `SKILL.md` 需含 YAML frontmatter：`name`（Skill 名）与 `description`（用途 + 触发场景，是豆包决定何时加载 Skill 的依据）；
- 需要脚本/资源时，放入 `scripts/`、`references/`、`assets/` 子目录；
- 有设计源稿时，以 `design-source.html` 与 `SKILL.md` 并列存放。

## License

保留所有权利。
