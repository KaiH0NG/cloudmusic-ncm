# 贡献指南

感谢你对本项目感兴趣！欢迎贡献代码。

## 🐛 提交 Bug

如果你发现了 Bug，请提交 Issue，包含以下信息：
- 操作系统和版本
- 复现步骤
- 预期行为 vs 实际行为
- 截图（如有）

## 💡 提出功能建议

欢迎提交功能建议！请描述：
- 你想要的功能
- 为什么需要这个功能
- 可能的实现方案

## 🔧 代码贡献

### 开发环境

```bash
# 克隆仓库
git clone https://github.com/Kai-403/ncm-batch-converter.git

# 安装依赖
pip install pyinstaller

# 运行源码测试
python ncm_converter.py "你的文件夹路径"
```

### 注意事项

1. 代码风格保持一致
2. 提交前先测试
3. 提交信息要清晰（英文）
4. 如果增加了新功能，更新 README.md

## 📝 提交格式

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Type 类型
- `feat`: 新功能
- `fix`: 修复 Bug
- `docs`: 文档更新
- `style`: 代码格式（不影响功能）
- `refactor`: 重构
- `test`: 测试相关

### 示例
```
feat: 添加进度显示功能

- 添加百分比进度条
- 支持取消转换

Closes #123
```

---

再次感谢你的贡献！ 💢