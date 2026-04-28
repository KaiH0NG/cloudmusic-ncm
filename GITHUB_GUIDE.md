# GitHub 上传详细步骤（小白版）

> 按照以下步骤操作，就能把你的项目上传到 GitHub 并发布 Release！

---

## 第一步：创建 GitHub 账号

如果你已经有账号，跳过此步骤。

1. 打开浏览器访问 **[github.com](https://github.com)**
2. 点击 **Sign up**（注册）
3. 输入你的邮箱、设置密码、取一个用户名
4. 验证邮箱（GitHub 会发一封邮件）
5. 完成！

---

## 第二步：创建仓库（Repository）

1. 登录 GitHub 后，点击右上角 **+** 按钮
2. 选择 **New repository**
3. 填写信息：
   - **Repository name**: `ncm-batch-converter`
   - **Description**: `网易云音乐NCM批量转MP3工具`
   - **Public** ← 选这个！（Public 才能让别人看到并点 star）
   - ✅ 不要勾选 "Add a README file"（我们已经有 README 了）
4. 点击 **Create repository**

创建完成后，你会看到一个页面，上面有你的仓库地址，类似：
```
https://github.com/Kai_403/ncm-batch-converter
```
（用户名不同可能不一样，记住你的地址）

---

## 第三步：推送代码到 GitHub

在页面上你会看到几行命令，找到**以 `…or push an existing repository from the command line` 开头的部分**，展开它，会显示类似：

```bash
git remote add origin https://github.com/Kai_403/ncm-batch-converter.git
git branch -M main
git push -u origin main
```

**复制这三行命令**，打开 Windows 的 **PowerShell** 或 **命令提示符**，粘贴并执行。

如果提示要输入用户名和密码：
- **Username**: 你的 GitHub 用户名
- **Password**: 你的 GitHub 密码（或者用 Personal Access Token）

> 💡 **注意**：如果你的 GitHub 开启了双因素认证，密码要用 Token 代替。
> Token 在 GitHub → Settings → Developer settings → Personal access tokens 生成。

---

## 第四步：发布 Release（赚 star 的关键！）

代码推送成功后，我们来发布一个版本，这样别人可以下载你的 exe 文件。

1. 进入你的仓库页面（例如 `https://github.com/Kai_403/ncm-batch-converter`）
2. 点击上方 **Releases**（在 Code 按钮右边）
3. 点击 **Draft a new release**
4. 填写信息：
   - **Tag version**: `v1.0.0`
   - **Release title**: `NCM批量转换器 v1.0.0`
   - **Describe this release**: 写点什么，比如"首个版本发布！拖拽文件夹即可批量转换 NCM 到 MP3"
5. 点击 **Attach binaries** 或把文件拖进去
   - 上传 `NCMConverter.exe`（在 `H:\NCMConverter.exe`）
   - 上传 `ncmdump.exe`（在 `H:\ncmdump.exe`）
6. 点击 **Publish release**

完成！✅

---

## 🎉 现在你有了什么

- ✅ 一个 GitHub 仓库
- ✅ 代码已推送
- ✅ 一个正式发布的 Release（别人可以下载 exe）
- ✅ 等待别人给你点 star ⭐

---

## 📊 验证是否成功

回到你的仓库页面，确认：
1. 可以看到所有文件（README.md, LICENSE, ncm_converter.py 等）
2. Releases 页面有 v1.0.0 版本
3. 能看到下载按钮

---

## 🔗 快捷访问

创建完仓库后，告诉我你的仓库地址，我帮你验证是否正确！