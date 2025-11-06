# TinaRen的AI作品集网站

一个现代化、酷炫的个人AI作品集展示网站，具有动态飞鸟背景、霓虹渐变效果和交互式卡片设计。

## ✨ 特色功能

- 🐦 **动态背景**：Vanta.js飞鸟动画效果
- 🌈 **霓虹渐变**：标题文字带有动态渐变和故障特效
- 💫 **交互设计**：卡片悬停时有发光和抬升效果
- 📱 **响应式布局**：完美适配手机、平板和电脑屏幕

## 📁 文件结构

```
tinaproject/
├── portfolio.html           # 主HTML文件
├── portfolio-style.css      # 样式文件
├── assets/
│   └── avatar.png          # 头像图片（需要自己添加）
└── vercel-portfolio.json   # Vercel部署配置
```

## 🚀 部署到Vercel

### 方法1：通过Vercel网站部署

1. 访问 [Vercel官网](https://vercel.com/)
2. 使用GitHub账号登录
3. 点击"New Project"
4. 选择你的项目仓库
5. 将 `vercel-portfolio.json` 重命名为 `vercel.json`
6. 点击"Deploy"

### 方法2：通过Vercel CLI部署

```bash
# 安装Vercel CLI
npm install -g vercel

# 登录Vercel
vercel login

# 在项目目录下运行
vercel

# 跟随提示完成部署
```

## 📝 使用说明

### 1. 准备头像图片

- 将你的头像图片命名为 `avatar.png`
- 放到 `assets/` 文件夹中
- 推荐尺寸：200x200像素或更高（正方形）
- 支持格式：PNG、JPG

### 2. 自定义内容

编辑 `portfolio.html` 文件，修改以下内容：

- 个人信息（联系方式、社交媒体）
- 视频链接（YouTube嵌入链接）
- 游戏和应用链接
- 项目描述文字

### 3. 自定义样式

编辑 `portfolio-style.css` 文件，可以调整：

- 颜色主题（修改渐变色值）
- 动画速度和效果
- 卡片样式和布局
- 字体大小和间距

## 🎨 颜色配置

主要颜色变量（在CSS中搜索这些颜色代码进行修改）：

- 主色调：`#ff00ff`（品红色）
- 辅色调：`#00ffff`（青色）
- 背景色：`#0a0a1f`（深蓝黑）

## 📱 响应式断点

- 桌面：> 768px
- 平板：768px - 481px
- 手机：≤ 480px

## 🔧 技术栈

- HTML5
- CSS3（动画、渐变、Flexbox、Grid）
- JavaScript
- [Vanta.js](https://www.vantajs.com/) - 动态背景
- [Three.js](https://threejs.org/) - 3D图形库

## 💡 自定义建议

### 添加更多视频

在 `portfolio.html` 中的视频网格部分添加：

```html
<div class="video-card">
    <iframe src="https://www.youtube.com/embed/你的视频ID"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen>
    </iframe>
</div>
```

### 添加更多项目卡片

在卡片网格部分添加：

```html
<a href="你的链接" target="_blank" class="game-card">
    <div class="card-icon">🎯</div>
    <h3>项目名称</h3>
    <p>项目描述</p>
    <div class="card-glow"></div>
</a>
```

### 更换Emoji图标

在 `card-icon` 中更换不同的emoji：
- 游戏类：🎮🎯🎲🎰🃏
- 工具类：🛠️📊📈📉⚙️
- 创意类：🎨🎭🎪🎬🎵

## 🐛 常见问题

### Q: 头像不显示？
A: 确保 `avatar.png` 文件在 `assets/` 文件夹中，路径正确。

### Q: 飞鸟动画不流畅？
A: 在 `portfolio.html` 底部的Vanta.js配置中，降低 `quantity` 值（鸟的数量）。

### Q: YouTube视频无法播放？
A: 检查视频链接格式，确保使用 `/embed/` 格式而非 `/watch?v=` 格式。

### Q: 手机端显示异常？
A: 清除浏览器缓存，确保CSS文件正确加载。

## 📄 许可证

此项目仅供个人使用和学习。

## 📧 联系方式

- 邮箱：renhong6@gmail.com
- 小红书：@Tina读书时间

---

**Powered by AI ✨**