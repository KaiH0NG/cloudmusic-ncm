# NCM批量转换器

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows-blue?style=for-the-badge" alt="Platform">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License">
  <img src="https://img.shields.io/github/stars/Kai-403/ncm-batch-converter?style=for-the-badge" alt="Stars">
</p>

> 把网易云音乐 VIP 下载的 `.ncm` 文件批量转换成 `.mp3` 文件。拖拽文件夹即可使用，无需复杂配置。

## 🎮 一键使用

**① 下载**
下载 `NCMConverter.exe` 和 `ncmdump.exe`，放在**同一目录**下。

**② 使用**
直接把存放 NCM 文件的**文件夹**拖到 `NCMConverter.exe` 上，搞定 ✅

```
拖文件夹到这里
    ↓
┌─────────────────────────────┐
│      NCMConverter.exe       │
└─────────────────────────────┘
    ↓
自动转换 → MP3 文件出现
```

## 📋 命令行用法

```bash
NCMConverter.exe "文件夹路径"
```

```bash
# 示例
NCMConverter.exe "H:\CloudMusic\VipSongsDownload"
```

## ⚙️ 工作原理

```
1. 扫描目标文件夹（含所有子文件夹）找出所有 .ncm 文件
2. 对每个文件调用 ncmdump.exe 进行转换
3. 转换后的 .mp3 保存到原文件同一目录
```

## ⚠️ 注意事项

- 转换出来的格式是 **MP3**（网易云 NCM 本身加密的就是 MP3）
- 转换后原 `.ncm` 文件**不会删除**，需要手动清理
- 仅支持 Windows 系统
- 需要 ncmdump.exe 放在同目录（已内置在 Release 中）

## 🔧 源码运行（开发者）

```bash
# 克隆项目
git clone https://github.com/Kai-403/ncm-batch-converter.git

# 安装 Python 依赖（仅转换脚本需要）
pip install pyinstaller

# 运行源码
python ncm_converter.py

# 打包成 exe
pyinstaller --onefile --name NCMConverter ncm_converter.py
```

## 📁 项目结构

```
ncm-batch-converter/
├── ncm_converter.py      # Python 源码
├── ncmdump.exe           # NCM 转换工具
├── NCMConverter.exe       # 打包好的可执行文件
├── README.md             # 说明文档
├── LICENSE               # MIT 开源许可证
├── CONTRIBUTING.md        # 贡献指南
├── CHANGELOG.md          # 更新日志
└── .gitignore            # Git 忽略规则
```

## 🛠️ 技术栈

| 组件 | 技术 |
|------|------|
| 转换工具 | [ncmdump](https://github.com/nICkname02/NCM批量下载转换) |
| 打包语言 | Python 3.x |
| 打包工具 | PyInstaller |
| 输出格式 | MP3 |

## 📝 更新日志

### v1.0 (2026-04-28)
- 初始版本发布
- 支持文件夹拖拽批量转换
- 内置 ncmdump.exe，无需额外下载

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件

---

⭐ 如果觉得好用，欢迎点个 Star！