# 贡献指南

感谢你对这个项目的关注！我们欢迎所有形式的贡献。

## 如何贡献

### 报告 Bug

如果你发现了 bug，请：

1. 查看 [Issues](https://github.com/kei-kez/ricoui-portfolio/issues) 确认该 bug 尚未被报告
2. 如果是一个新的 bug，请创建一个新的 Issue，包含：
   - 清晰的问题描述
   - 复现步骤
   - 预期行为
   - 实际行为
   - 截图（如果有）
   - 环境信息（浏览器、操作系统等）

### 提出新功能

如果你有改进建议或新功能想法：

1. 查看现有 Issues 确认没有类似提议
2. 创建一个新的 Feature Request Issue，描述：
   - 功能描述
   - 使用场景
   - 可能的实现方案（可选）

### 提交代码

1. **Fork 项目**
   ```bash
   git clone https://github.com/your-username/ricoui-portfolio.git
   cd ricoui-portfolio
   ```

2. **创建分支**
   ```bash
   git checkout -b feature/your-feature-name
   # 或
   git checkout -b fix/your-bug-fix
   ```

3. **安装依赖**
   ```bash
   pnpm install
   ```

4. **进行修改**
   - 编写代码
   - 确保代码通过检查：`pnpm check`
   - 测试你的修改

5. **提交更改**
   ```bash
   git add .
   git commit -m "feat: 添加新功能描述"
   # 或
   git commit -m "fix: 修复bug描述"
   ```

   提交信息请遵循 [Conventional Commits](https://www.conventionalcommits.org/) 规范：
   - `feat:` 新功能
   - `fix:` Bug 修复
   - `docs:` 文档更新
   - `style:` 代码格式调整（不影响功能）
   - `refactor:` 代码重构
   - `perf:` 性能优化
   - `test:` 测试相关
   - `chore:` 构建/工具相关

6. **推送并创建 Pull Request**
   ```bash
   git push origin feature/your-feature-name
   ```

   然后在 GitHub 上创建 Pull Request。

## 代码规范

- 使用 Biome 进行代码检查和格式化
- 运行 `pnpm check` 确保代码符合规范
- 保持代码简洁、可读
- 添加必要的注释

## 开发环境

- Node.js >= 18
- pnpm (推荐) 或 npm/yarn
- 现代浏览器（Chrome、Firefox、Safari、Edge）

## 测试

在提交 PR 前，请确保：

- [ ] 代码通过 `pnpm check`
- [ ] 在本地运行 `pnpm dev` 测试正常
- [ ] 构建通过 `pnpm build`
- [ ] 测试了不同的浏览器和设备

## 问题？

如果遇到问题，可以：

- 查看 [Issues](https://github.com/kei-kez/ricoui-portfolio/issues)
- 创建新的 Issue 提问
- 联系维护者：hello@ricoui.com

再次感谢你的贡献！🎉

