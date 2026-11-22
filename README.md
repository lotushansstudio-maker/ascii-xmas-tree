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

没有摄像头时可按键盘 `0`–`5` 切换，手机上点屏幕切换。单手左右移动可以拨动树的旋转。

## 技术
- 手势识别：[MediaPipe Hand Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker)（浏览器端，21 个手部关键点）
- 渲染：一个很小的「字符 3D 渲染器」：约 4 万个 3D 采样点 → 旋转 / 透视投影 → z-buffer → 光照 → 按亮度选字符，画到固定的字符网格上
- 细节：生长时上升的发光切面、左侧打光的分层树冠、挂球、彩虹灯带、光芒星、透视地面、线条驯鹿、比心爆雪、柔光
- 单个 `index.html`，无需构建

## 本地运行
```
python3 -m http.server 8000
# 打开 http://localhost:8000
```
