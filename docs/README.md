# SentencePlayer MCP - GitHub Pages

这个目录包含 SentencePlayer MCP 的 GitHub Pages 网站文件。

## 📁 目录结构

```
docs/
├── index.html              # 主页
├── css/
│   └── style.css          # 样式文件
├── js/
│   └── main.js            # JavaScript
└── images/
    ├── icon.png           # 应用图标 (需要添加)
    ├── logo.png           # Logo (需要添加)
    ├── og-image.png       # 社交媒体分享图片 (需要添加)
    └── screenshots/       # 应用截图 (需要添加)
        ├── main.png
        ├── test.png
        └── logs.png
```

## 🚀 部署步骤

### 1. 准备图片资源

你需要添加以下图片到相应目录：

- `docs/images/icon.png` - 应用图标 (建议 512x512px)
- `docs/images/logo.png` - Logo (建议透明背景 PNG)
- `docs/images/og-image.png` - 社交分享图片 (建议 1200x630px)
- `docs/images/screenshots/main.png` - 主界面截图
- `docs/images/screenshots/test.png` - 测试界面截图
- `docs/images/screenshots/logs.png` - 日志界面截图

### 2. 创建 GitHub 仓库

```bash
# 在 GitHub 网站上创建新仓库: SentencePlayerMCP
# 然后在本地：

cd 你的项目目录
git init
git add .
git commit -m "Initial commit with GitHub Pages"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/SentencePlayerMCP.git
git push -u origin main
```

### 3. 启用 GitHub Pages

1. 进入仓库设置: Settings → Pages
2. Source: Deploy from a branch
3. Branch: main
4. Folder: /docs
5. Save

### 4. 访问网站

几分钟后访问：
```
https://YOUR_USERNAME.github.io/SentencePlayerMCP/
```

## ✏️ 自定义修改

### 更新 GitHub 链接

在 `index.html` 中搜索并替换：
- `YOUR_USERNAME` → 你的 GitHub 用户名

### 更新 App Store 链接

在 `index.html` 中找到 "Download on the App Store" 按钮，添加实际的 App Store 链接。

### 修改配色

在 `style.css` 中的 `:root` 部分修改颜色变量：

```css
:root {
    --primary-color: #007AFF;    /* 主色调 */
    --secondary-color: #5856D6;  /* 次要颜色 */
    /* ... */
}
```

## 📊 图片规格建议

### 应用图标 (icon.png)
- 尺寸: 512x512px 或 1024x1024px
- 格式: PNG (透明背景)
- 用途: 导航栏、favicon

### Logo (logo.png)
- 尺寸: 宽度 300-500px
- 格式: PNG (透明背景)
- 用途: 页脚、社交分享

### 截图 (screenshots/*.png)
- 尺寸: 1280x800px 或更大
- 格式: PNG 或 JPG
- 用途: 功能展示
- 建议: 添加设备框架使其更美观

### OG Image (og-image.png)
- 尺寸: 1200x630px
- 格式: PNG 或 JPG
- 用途: 社交媒体分享预览

## 🎨 使用工具生成图片

### 截图美化
- [Screely](https://screely.com/) - 添加渐变背景
- [Shotsnapp](https://shotsnapp.com/) - 添加设备框架
- [Screenshot.rocks](https://screenshot.rocks/) - 美化截图

### 图标设计
- [Canva](https://www.canva.com/) - 在线设计
- [Figma](https://www.figma.com/) - 专业设计工具

## 📱 测试清单

- [ ] 所有链接正常工作
- [ ] 图片加载正确
- [ ] 移动端显示正常
- [ ] 社交分享卡片正确显示
- [ ] GitHub 链接指向正确仓库
- [ ] App Store 链接正确（上架后）

## 🔧 本地测试

```bash
# 使用 Python 简单服务器
cd docs
python3 -m http.server 8000

# 访问 http://localhost:8000
```

或使用 [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) VS Code 扩展。

## 📈 添加分析（可选）

在 `</head>` 前添加 Google Analytics：

```html
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🎯 SEO 优化

已包含的 SEO 优化：
- ✅ Meta 描述
- ✅ 关键词
- ✅ Open Graph 标签
- ✅ Twitter Card 标签
- ✅ 语义化 HTML
- ✅ 响应式设计

## 📞 支持

如有问题，请在 GitHub 仓库创建 Issue。

---

**注意**: 记得在上传到 GitHub 前添加所有必需的图片！
