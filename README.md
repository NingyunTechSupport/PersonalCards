<div align="center">
  <h1>寧雲技术支持中心 · 个人名片组合</h1>
  <p><strong>红蓝白配色 · 纯静态 · 粒子动画 · 响应式设计</strong></p>
  <p>
    <a href="https://card.ningyun.sd.cn"><img src="https://img.shields.io/badge/访问-名片导航页-DC2626?style=flat-square" alt="名片导航页"></a>
    <a href="https://card.ningyun.sd.cn/ny/"><img src="https://img.shields.io/badge/名片-寧雲-1E3A8A?style=flat-square" alt="寧雲名片"></a>
    <a href="https://card.ningyun.sd.cn/zhh/"><img src="https://img.shields.io/badge/名片-之槐-FB7299?style=flat-square" alt="之槐名片"></a>
  </p>
</div>

---

## 项目简介

本项目是寧雲技术支持中心成员的个人名片集合，包含一个**暗色粒子导航页**和两张风格统一的**个人名片**。所有页面均为纯静态 HTML，部署于 Cloudflare Pages，通过 `card.ningyun.sd.cn` 域名访问。

### 页面一览

| 页面 | 路径 | 说明 |
|------|------|------|
| 名片导航 | `/` | 暗色主题 + Canvas 粒子动画，两个入口卡片 |
| 寧雲名片 | `/ny/` | 负责人名片，红蓝白亮色调，含微信二维码弹窗、GitHub/B站二次确认跳转 |
| 之槐名片 | `/zhh/` | 成员名片，风格与寧雲统一，含 B 站二次确认及价目表全屏查看 |

---

## 在线地址

- **名片导航页**：https://card.ningyun.sd.cn
- **寧雲名片**：https://card.ningyun.sd.cn/ny/
- **之槐名片**：https://card.ningyun.sd.cn/zhh/

---

## 技术特点

- **纯静态 HTML/CSS/JS**，无框架依赖
- **Canvas 粒子动画**：红蓝白配色粒子带连线效果（导航页）
- **CSS 浮动光晕**：三色径向渐变光晕持续浮动（名片页）
- **红蓝白统一配色**：红色 `#DC2626` + 蓝色 `#1E3A8A` + 白色
- **交互细节**：悬停左移、左侧红白竖杠动画、图标变色、红蓝交替状态点
- **弹窗系统**：微信二维码弹窗（绿色主题）、外部链接二次确认弹窗（平台强调色）
- **响应式设计**：适配桌面端与移动端，含汉堡菜单
- **Cloudflare Pages 部署**：全球 CDN，零成本托管

---

## 目录结构

```
.
├── index.html                # 名片导航页（暗色·粒子动画）
├── ny/
│   ├── index.html            # 寧雲个人名片
│   ├── avatar.jpg            # 寧雲头像
│   └── wechat-qr.jpg         # 寧雲微信二维码
└── zhh/
    ├── index.html            # 之槐个人名片
    ├── avatar.jpg            # 之槐头像
    └── price-list.jpg        # 之槐价目表（可选）
```

---

## 快速部署

1. **Fork 或克隆本仓库**
   ```bash
   git clone https://github.com/NingyunTechSupport.git
   cd NingyunTechSupport
   git checkout card   # 切换到 card 分支
   ```

2. **修改个人信息**
   - 替换 `ny/avatar.jpg` 和 `zhh/avatar.jpg` 为真实头像
   - 替换 `ny/wechat-qr.jpg` 为微信二维码
   - 在 HTML 中搜索邮箱、QQ、链接等并替换

3. **部署到 Cloudflare Pages**
   - 登录 Cloudflare → Workers & Pages → 创建 → Pages
   - 连接 Git 仓库，选择 `card` 分支
   - 构建命令：*留空*
   - 输出目录：`/`
   - 绑定自定义域名 `card.ningyun.sd.cn`

---

## 自定义指南

### 修改个人信息

在对应的 `index.html` 中搜索并替换：

| 信息项 | 寧雲名片位置 | 之槐名片位置 |
|--------|-------------|-------------|
| 姓名 | `ny/index.html` 中 `profile-name` | `zhh/index.html` 中 `profile-info h1` |
| 邮箱 | 搜索 `nypub1916@ningyun.top` | 搜索 `563602369@qq.com` |
| QQ | 搜索 `3665881428` | 搜索 `563602369` |
| B站链接 | 搜索 `1574036934` | 搜索 `2060315070` |
| GitHub | 搜索 `NingyunTechSupport` | — |

### 替换图片

| 文件 | 用途 | 建议尺寸 |
|------|------|----------|
| `ny/avatar.jpg` | 寧雲头像 | 400×400 |
| `ny/wechat-qr.jpg` | 寧雲微信二维码 | 400×400 |
| `zhh/avatar.jpg` | 之槐头像 | 400×400 |
| `zhh/price-list.jpg` | 之槐价目表 | 800×1200 |

---

## 成员信息

| 姓名 | 角色 | 技术方向 | 名片链接 |
|------|------|----------|----------|
| 寧雲 | 负责人·技术支持 | Windows系统定制、优化与软件部署 | [`/ny/`](https://card.ningyun.sd.cn/ny/) |
| 之槐 | 软件部署·文档设计 | Windows系统重装、美化与文字处理 | [`/zhh/`](https://card.ningyun.sd.cn/zhh/) |

---

## 相关项目

- **官网主页**：https://ningyun.icu （[GitHub 仓库](https://github.com/NingyunTechSupport)）
- **柠檬镇服务器存档**：`lmtn.pages.dev`

---

## 许可证

本项目仅供寧雲技术支持中心及其成员使用，保留所有权利。
第三方可参考设计，请勿直接商业使用。

---

© 2026 寧雲技术支持中心. All rights reserved.
