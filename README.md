# 🔫 3D 射击游戏

一个纯 HTML 的 **3D 第一人称射击小游戏**，使用 [Three.js](https://threejs.org/) 构建。
**无需任何构建工具**，单个 `index.html` 文件即可运行。

![Three.js](https://img.shields.io/badge/Three.js-r128-fffd69) ![Pure HTML](https://img.shields.io/badge/Pure-HTML%20%2B%20JS-4c1)

---

## 🎮 游戏特色

- ✅ **真正的 3D 场景** —— 草地、掩体、树木、天空雾效
- ✅ **第一人称视角** —— 鼠标控制视角，逼真的后坐力动画
- ✅ **射线检测射击** —— 快速精准的命中判定 + 弹道轨迹
- ✅ **AI 敌人** —— 会追踪玩家、绕过掩体、接触造成伤害
- ✅ **难度递增** —— 敌人数量和速度随时间增加
- ✅ **合成音效** —— 使用 Web Audio API，无需音频文件
- ✅ **完整 HUD** —— 生命、得分、击杀数、存活时间

## 🕹 操作说明

| 操作 | 按键 |
|------|------|
| 移动 | `W` `A` `S` `D` |
| 视角 | 鼠标移动 |
| 射击 | 鼠标左键 |
| 奔跑 | `Shift` |
| 释放鼠标 | `Esc` |

## 🚀 如何运行

### 方法一：直接打开（最快）
1. 用浏览器打开 `index.html` 文件
2. 点击「开始游戏」
3. 鼠标会被自动锁定，移动鼠标即可转动视角

> ⚠️ 由于浏览器安全限制，`requestPointerLock`（鼠标锁定）需要通过用户点击触发，所以请先点击开始按钮。

### 方法二：GitHub Pages（可分享链接）
本仓库已托管在 GitHub 上，可以开启 Pages 发布：

1. 进入仓库设置 → Pages
2. 来源选择 `main` 分支，根目录 `/`
3. 保存后等待几分钟，即可通过 `https://<username>.github.io/3d-shooter-game/` 访问

### 方法三：本地服务器
```bash
# 任意静态服务器即可，例如：
python -m http.server 8000
# 然后访问 http://localhost:8000
```

## 🛠 技术栈

- [Three.js](https://threejs.org/) —— 3D 渲染引擎（CDN 引入）
- Web Audio API —— 音效合成
- 原生 JavaScript ES6+

## 🎯 玩法提示

- 利用**掩体（灰色方块）**躲避敌人
- 敌人血量 3 点，快速连击可击杀
- 击杀 +100 分，活越久敌人越强
- 被敌人碰到会扣血，血量归零游戏结束

## 📁 项目结构

```
3d-shooter-game/
├── index.html   # 游戏全部代码（HTML + CSS + JS）
└── README.md    # 说明文档
```

## 🧩 可扩展方向

- [ ] 增加更多武器（手枪、步枪、狙击枪）
- [ ] 增加背包 / 道具系统
- [ ] 增加波次（wave）机制
- [ ] 增加排行榜（localStorage）
- [ ] 移动端触控支持

---

纯前端实现，无需后端，开箱即用。玩得开心！🎉
