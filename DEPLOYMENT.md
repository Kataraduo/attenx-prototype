
# AttenX 部署指南

本文档提供了将AttenX原型部署到公开可访问网站的详细步骤。您可以选择GitHub Pages或Netlify进行部署，两者都提供免费的静态网站托管服务。

## 方法一：使用GitHub Pages部署

### 步骤1：创建GitHub仓库

1. 登录您的GitHub账户（如果没有，请在[github.com](https://github.com)注册）
2. 点击右上角的"+"图标，选择"New repository"
3. 仓库名称建议使用：`attenx-prototype`
4. 选择公开(Public)仓库
5. 点击"Create repository"

### 步骤2：上传项目文件

**使用Git命令行：**

```bash
# 在项目目录中初始化Git仓库
git init

# 添加所有文件到暂存区
git add .

# 提交更改
git commit -m "初始提交 - AttenX原型"

# 添加远程仓库（替换YOUR-USERNAME为您的GitHub用户名）
git remote add origin https://github.com/YOUR-USERNAME/attenx-prototype.git

# 推送到GitHub
git push -u origin main
```

**或使用GitHub Desktop：**

1. 下载并安装[GitHub Desktop](https://desktop.github.com/)
2. 登录您的GitHub账户
3. 添加本地仓库（选择AttenX项目文件夹）
4. 提交所有更改
5. 发布仓库到GitHub

### 步骤3：启用GitHub Pages

1. 在GitHub仓库页面，点击"Settings"
2. 滚动到"Pages"部分
3. 在"Source"下，选择"main"分支
4. 点击"Save"
5. 等待几分钟，您的网站将在以下URL可用：`https://YOUR-USERNAME.github.io/attenx-prototype/`

## 方法二：使用Netlify部署

### 步骤1：创建Netlify账户

1. 访问[netlify.com](https://www.netlify.com/)并注册账户（可以使用GitHub账户登录）

### 步骤2：部署网站

**从GitHub部署：**

1. 在Netlify控制面板中，点击"New site from Git"
2. 选择"GitHub"作为Git提供商
3. 授权Netlify访问您的GitHub账户
4. 选择您的AttenX仓库
5. 保持默认设置，点击"Deploy site"

**或直接上传文件：**

1. 在Netlify控制面板中，点击"Sites"部分
2. 将整个项目文件夹拖放到指定区域
3. 等待上传和部署完成

### 步骤3：自定义域名（可选）

1. 在站点控制面板中，点击"Domain settings"
2. 您可以使用Netlify提供的免费子域名，或设置自定义域名

## 更新网站

无论您选择哪种部署方法，当您对原型进行更改后，只需将更新后的文件推送到GitHub仓库，网站将自动更新。

## 注意事项

- 确保所有资源（图片、CSS、JavaScript）使用相对路径
- 检查所有链接是否正确工作
- 测试部署后的网站在不同设备和浏览器上的表现

## 帮助与支持

如果您在部署过程中遇到任何问题，请参考：

- [GitHub Pages文档](https://docs.github.com/cn/pages)
- [Netlify文档](https://docs.netlify.com/)