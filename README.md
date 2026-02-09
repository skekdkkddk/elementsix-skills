# 🛠️ ElementSix Skills

ElementSix 的 Claude Code Skills 合集 Marketplace。

## 📦 包含的 Skills

| Skill | 描述 | 版本 |
|-------|------|------|
| [seedance-storyboard](./seedance-storyboard) | 将任何想法转换成即梦 Seedance 2.0 专业分镜提示词 | 1.0.0 |
| [my-commit](./my-commit) | Git 提交助手，帮助生成规范的提交信息 | 1.0.0 |

## 🚀 安装方法

### 添加 Marketplace

```bash
/plugin marketplace add elementsix/elementsix-skills
```

### 安装 Skills

```bash
# 安装 Seedance Storyboard
/plugin install seedance-storyboard@elementsix-skills

# 安装 My Commit
/plugin install my-commit@elementsix-skills
```

## 📖 使用 Skills

安装后，直接使用命令：

```bash
# 使用 Seedance Storyboard
/seedance-storyboard

# 使用 My Commit
/my-commit
```

## 🏗️ 项目结构

```
elementsix-skills/
├── .claude-plugin/
│   └── marketplace.json      # Marketplace 配置
├── seedance-storyboard/      # Skill 1
│   ├── SKILL.md
│   ├── examples/
│   ├── templates/
│   └── ...
└── my-commit/                # Skill 2
    └── SKILL.md
```

## 📝 添加新 Skill

1. 在根目录创建新文件夹 `new-skill/`
2. 添加 `SKILL.md` 文件
3. 更新 `.claude-plugin/marketplace.json`
4. 提交并推送

## 📄 许可证

MIT License
