# 吟诵教程文档部署指南

## 本地预览

由于我们没有全局安装docsify-cli，您可以使用以下方法在本地预览文档：

### 方法1：使用Python的简易HTTP服务器

如果您的电脑上安装了Python，可以使用Python自带的HTTP服务器：

```bash
# Python 3.x
python -m http.server

# 然后在浏览器中访问 http://localhost:8000
```

### 方法2：使用VS Code的Live Server插件

如果您使用VS Code，可以安装Live Server插件，然后右键点击index.html文件，选择"Open with Live Server"。

## 部署到GitHub Pages

### 步骤1：创建GitHub仓库

1. 登录您的GitHub账号
2. 创建一个新的仓库，命名可以是`yinsong-tutorial`或其他您喜欢的名称
3. 选择公开或私有仓库（GitHub Pages对公开仓库是免费的）

### 步骤2：上传文件

将以下文件上传到您的GitHub仓库：
- index.html
- README.md
- _sidebar.md
- _coverpage.md
- .nojekyll
- 所有的Markdown教程文件（01 - ... 到39 - ...）

### 步骤3：开启GitHub Pages

1. 进入仓库的Settings页面
2. 在左侧菜单中选择"Pages"
3. 在"Source"部分，从"Branch"下拉菜单中选择主分支（通常是main或master），然后选择"/(root)"目录
4. 点击"Save"按钮
5. 等待几分钟，GitHub Pages就会部署您的文档网站

### 步骤4：访问您的文档网站

部署完成后，您可以通过GitHub提供的URL访问您的文档网站，格式通常是：`https://[您的GitHub用户名].github.io/[仓库名称]`

## 更新文档

要更新文档，只需修改或添加对应的Markdown文件，然后推送到GitHub仓库即可。GitHub Pages会自动更新您的网站。