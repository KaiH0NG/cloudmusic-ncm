# NCM Batch Converter

把网易云音乐 VIP 下载的 `.ncm` 文件批量转换成 `.mp3` 文件。拖拽文件夹即可使用，无需复杂配置。

## 🎮 使用方法

**方法1：拖拽（最简单）**
```
直接把文件夹拖到 NCMConverter.exe 上
```

**方法2：命令行**
```bash
NCMConverter.exe "文件夹路径"
```

## 📋 示例

```
NCMConverter.exe "C:\Users\YourName\Music\VipSongs"
```

## ⚙️ 工作原理

1. 扫描目标文件夹（含子文件夹）找出所有 `.ncm` 文件
2. 对每个文件调用 `ncmdump.exe` 进行转换
3. 转换后的 `.mp3` 保存到**原文件同目录**

## 📦 下载

直接下载 Releases 中的 `NCMConverter.exe` 即可使用（已内置 ncmdump.exe）。

## ⚠️ 注意事项

- 转换出来的格式是 **MP3**（网易云 NCM 本身加密的就是 MP3）
- `ncmdump.exe` 已内置，无需额外下载
- 仅支持 Windows 系统

## 🔧 依赖

- Python 3.x（源码运行）
- [ncmdump](https://github.com/nICkname02/NCM批量下载转换)（已内置）

## 📁 项目结构

```
ncm-batch-converter/
├── ncm_converter.py     # 源码
├── ncmdump.exe          # 转换工具（已内置）
├── NCMConverter.exe     # 打包好的可执行文件
└── README.md            # 说明文档
```

## ⭐ 如果觉得好用，欢迎点个 Star！