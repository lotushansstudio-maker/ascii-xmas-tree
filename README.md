# ASCII Xmas Tree · 手势圣诞树 🎄

用摄像头和手势，让几千个 ASCII 字符长成一棵圣诞树。

**在线体验：** https://lotushansstudio-maker.github.io/ascii-xmas-tree/

| 手势 | 效果 |
|---|---|
| ✊ 握拳 | 重置 |
| 🖐 张开手掌 | 长出圣诞树 |
| ☝️ 竖食指 | 点亮星星 |
| ✌️ 比耶 | 挂上彩灯 |
| 🙌 双手张开 | 礼物 |
| 🫶 双手比心 | 驯鹿 |

没有摄像头时可按键盘 `0`–`5` 切换。

## 技术
- 手势识别：[MediaPipe Hand Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker)（浏览器端，21 个手部关键点）
- 渲染：原生 Canvas 2D，约 3000 个字符粒子，在 3D 圆锥上旋转并做透视投影
- 单个 `index.html`，无需构建

## 本地运行
```
python3 -m http.server 8000
# 打开 http://localhost:8000
```
