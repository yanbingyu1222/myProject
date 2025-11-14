# Git设置和GitHub Pages部署指南

## 📋 完整步骤

### 1. 配置Git用户信息
```powershell
& "C:\Program Files\Git\bin\git.exe" config --global user.name "你的用户名"
& "C:\Program Files\Git\bin\git.exe" config --global user.email "你的邮箱"
```

### 2. 添加文件到Git
```powershell
& "C:\Program Files\Git\bin\git.exe" add .
& "C:\Program Files\Git\bin\git.exe" commit -m "初始提交：生日祝福网页"
```

### 3. 创建GitHub仓库
1. 访问 [github.com](https://github.com)
2. 点击右上角的 "+" → "New repository"
3. 仓库名称：`birthday-wishes`（或其他你喜欢的名字）
4. 选择 "Public"（必须公开才能使用GitHub Pages）
5. 不要勾选"Add a README file"（我们已经有了）
6. 点击"Create repository"

### 4. 连接远程仓库并推送
创建仓库后，GitHub会显示命令，类似：
```powershell
& "C:\Program Files\Git\bin\git.exe" remote add origin https://github.com/你的用户名/birthday-wishes.git
& "C:\Program Files\Git\bin\git.exe" branch -M main
& "C:\Program Files\Git\bin\git.exe" push -u origin main
```

### 5. 启用GitHub Pages
1. 在GitHub仓库页面，点击"Settings"
2. 在左侧菜单找到"Pages"
3. 在"Build and deployment"下，选择"Deploy from a branch"
4. "Branch"选择"main"，文件夹选择"/ (root)"
5. 点击"Save"

### 6. 获取链接
等待几分钟后，你的网页就可以通过以下链接访问：
- 🎂 **生日快乐页面**: `https://你的用户名.github.io/birthday-wishes/生日快乐.html`
- 🎉 **生日祝福页面**: `https://你的用户名.github.io/birthday-wishes/生日祝福.html`

## 🚀 快速命令复制粘贴

将以下命令复制到PowerShell中执行（记得替换用户名和邮箱）：

```powershell
# 配置用户信息
& "C:\Program Files\Git\bin\git.exe" config --global user.name "你的GitHub用户名"
& "C:\Program Files\Git\bin\git.exe" config --global user.email "你的邮箱地址"

# 添加文件
& "C:\Program Files\Git\bin\git.exe" add .

# 提交
& "C:\Program Files\Git\bin\git.exe" commit -m "添加生日祝福网页"

# 添加远程仓库（创建GitHub仓库后替换为你的地址）
& "C:\Program Files\Git\bin\git.exe" remote add origin https://github.com/你的用户名/birthday-wishes.git

# 推送到GitHub
& "C:\Program Files\Git\bin\git.exe" branch -M main
& "C:\Program Files\Git\bin\git.exe" push -u origin main
```

## 💡 提示
- 如果推送时要求输入用户名和密码，请使用GitHub Personal Access Token而不是密码
- 获取Token：GitHub Settings → Developer settings → Personal access tokens → Generate new token
- Token需要勾选"repo"权限

## 🎯 完成后
你就可以分享链接给朋友了！链接格式：
`https://你的用户名.github.io/birthday-wishes/生日快乐.html`