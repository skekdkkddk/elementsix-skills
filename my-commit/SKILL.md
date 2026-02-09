---
name: my-commit
description: 创建规范的 Git 提交信息。当用户说"提交代码"、"commit"、"创建提交"时使用。
disable-model-invocation: true
allowed-tools: Read, Bash
---

# 创建 Git 提交

帮助用户创建规范的 Git 提交。

## 工作流程

1. 检查当前的 Git 状态
   ```bash
   git status
   git diff --stat
   ```

2. 如果有未暂存的更改，询问用户要提交哪些文件

3. 分析更改内容，建议合适的提交类型：
   - `feat`: 新功能
   - `fix`: 修复 bug
   - `docs`: 文档更新
   - `style`: 代码格式调整
   - `refactor`: 重构
   - `test`: 测试相关
   - `chore`: 构建/工具相关

4. 生成提交信息，格式：`<type>: <description>`

5. 执行提交：
   ```bash
   git add <选择的文件>
   git commit -m "<提交信息>"
   ```

## 示例提交信息

- feat: 添加用户登录功能
- fix: 修复导航栏样式问题
- docs: 更新 README 安装说明
- refactor: 优化数据库查询逻辑
