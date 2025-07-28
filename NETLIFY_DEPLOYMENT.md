# 部署支票生成器到 Netlify

这个项目已经配置好可以直接部署到 Netlify。

## 部署步骤

### 方法一：通过 Git 仓库部署（推荐）

1. 将项目推送到 GitHub、GitLab 或 Bitbucket
2. 登录 [Netlify](https://netlify.com)
3. 点击 "New site from Git"
4. 选择你的 Git 提供商并授权
5. 选择这个项目的仓库
6. Netlify 会自动检测到 `netlify.toml` 配置文件
7. 点击 "Deploy site"

### 方法二：手动拖拽部署

1. 登录 [Netlify](https://netlify.com)
2. 在仪表板中找到 "Sites" 部分
3. 将整个项目文件夹拖拽到 "Want to deploy a new site without connecting to Git? Drag and drop your site output folder here" 区域
4. Netlify 会自动部署你的网站

## 项目文件说明

- `index.html` - 主页面（支票生成器）
- `netlify.toml` - Netlify 部署配置文件
- 其他文件 - 项目的其他资源和工具

## 配置说明

`netlify.toml` 文件包含了以下配置：

- **发布目录**: `./` （当前目录）
- **构建命令**: 无需构建，直接部署静态文件
- **安全头部**: 包含了基本的安全配置
- **缓存策略**: HTML 文件不缓存，CSS/JS 文件长期缓存

## 访问你的网站

部署完成后，Netlify 会提供一个随机的 URL（如 `https://amazing-name-123456.netlify.app`）。

你可以：
- 使用这个 URL 直接访问
- 在 Netlify 仪表板中自定义域名
- 绑定你自己的域名

## 注意事项

- 这是一个纯前端应用，所有功能都在浏览器中运行
- 不需要服务器端处理
- 支票数据不会被保存到服务器，仅在本地浏览器中处理

## 功能特性

- 智能分期计算
- 自定义支付计划
- 日期选择器
- 货币格式化
- 响应式设计
- 支票预览和打印功能