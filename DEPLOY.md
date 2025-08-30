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

将所有文档文件上传到GitHub仓库。确保包含以下关键文件：
- index.html
- README.md
- _sidebar.md
- _coverpage.md
- .nojekyll
- 所有Markdown教程文件
- Image文件夹（包含logo图片）

### 步骤3：开启GitHub Pages功能

1. 进入仓库的"Settings"页面
2. 点击左侧菜单的"Pages"
3. 在"Source"选项中，选择"main"分支和根目录（/root）
4. 点击"Save"按钮

### 步骤4：访问您的网站

等待几分钟后，您的网站将可以通过GitHub Pages提供的URL访问，格式通常为：`https://<您的GitHub用户名>.github.io/<仓库名>/`

## 注意事项

- 如果您修改了文档内容，需要将更改提交并推送到GitHub仓库，然后等待GitHub Pages更新
- 确保所有链接都使用正确的URL编码（特别是包含空格的文件名）
- .nojekyll文件很重要，它告诉GitHub Pages不要使用Jekyll处理这些文件，这对于docsify网站是必需的
