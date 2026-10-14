<div align="center">

# 🎬 coordinate-camera-control-designer

## 把打斗写成 [L,T,W,H]：坐标控住乱飞的镜头
## Fights as [L,T,W,H]: coordinates stop the camera flying blind

📮 **商务合作 / Business：wow.vip@foxmail.com**
🎬 **抖音 / Douyin：[v.douyin.com/07EjIDGVErY](https://v.douyin.com/07EjIDGVErY/)**

</div>

---

## 🇨🇳 中文

高速动作片最常见的失败是观众看不清谁打谁、镜头乱飞。它把「角色从 A 点到 B 点」「闪现攻击」「撞击飞出」「跑酷追逐」拆成四层坐标：主体框、相机关注框、目标框与事件框，再配可解释的速度函数，而不是只写「很快」。先出 16:9 场景运动轨迹总图和黑白线稿 3×3 总分镜图，再给每个 cut 一条带 [L,T,W,H] 的视频提示词。路径图、箭头、坐标框、cut 编号只属于规划层，最终画面明确禁止它们入画。

### ✨ 能做什么

- 四层坐标体系：subject_box、camera_focus、target_box / event_box、speed_curve，先建体系再写提示词
- 人物坐标与相机坐标严格分离：相机可跟随、领先跟随、环绕、俯视跟随、拉远、推近、低角度上摇、斜切
- 8 种可解释速度函数：linear、ease-in、ease-out、ease-in-out、burst-stop、stop-burst、peak-mid、impact-freeze
- 默认拆 9 个 cut，交付坐标运镜分镜表：镜头类型、主体/事件、坐标控制、镜头运动、节奏、速度曲线
- 生成 16:9 场景运动轨迹总图 + 黑白线稿 3×3 总分镜图（C1-C9 对应 9 个 cut），必要时再加一张无箭头、无编号的干净场景参考图专供视频生成
- 缺框选界面时用九宫格估算坐标（左上 [L=0.05,T=0.05,W=0.20,H=0.25] 等 9 个基准位置）

### 📦 包含的技能

- `coordinate-camera-control-designer` —— 见 [`coordinate-camera-control-designer/SKILL.md`](coordinate-camera-control-designer/SKILL.md)

### 🚀 安装

```bash
git clone https://github.com/yzsp-studio/coordinate-camera-control-designer.git
cp -r coordinate-camera-control-designer/* "$DSH_HOME/skills/"
```

> 技能是**纯文本说明**（`SKILL.md` + `references/`），零依赖、零 API key，用你当前 agent 的会话额度。

---

## 🇬🇧 English

The most common failure of a fast action shot is that nobody can tell who hit whom while the camera flies around. This turns runs from A to B, flash attacks, impact knockbacks and parkour chases into four coordinate layers, subject box, camera focus box, target box and event box, paired with explainable speed curves instead of the word fast. You get a 16:9 scene motion-path overview and a monochrome 3x3 master storyboard, then one coordinate-carrying video prompt per cut. Arrows, coordinate boxes and cut numbers belong to the planning layer and are explicitly barred from the final frame.

### ✨ What it does

- Four coordinate layers built before any prompt: subject_box, camera_focus, target_box/event_box and speed_curve
- Subject coordinates kept strictly separate from camera coordinates: follow, lead-follow, orbit, top-down, pull-back, push-in, tilt-up, dutch-shift
- Eight explainable speed functions: linear, ease-in, ease-out, ease-in-out, burst-stop, stop-burst, peak-mid and impact-freeze
- Nine cuts by default, delivered as a coordinate storyboard table of shot type, subject, coordinates, camera move, beat and speed curve
- A 16:9 motion-path overview plus a single monochrome 3x3 master storyboard mapping C1-C9 to nine cuts, with an optional clean scene reference that carries no arrows or numbering
- Nine-grid coordinate estimation presets when no framing tool exists, such as top-left at [L=0.05,T=0.05,W=0.20,H=0.25]

### 📦 Skills included

- `coordinate-camera-control-designer` — [`coordinate-camera-control-designer/SKILL.md`](coordinate-camera-control-designer/SKILL.md)

### 🚀 Install

```bash
git clone https://github.com/yzsp-studio/coordinate-camera-control-designer.git
cp -r coordinate-camera-control-designer/* "$DSH_HOME/skills/"
```

> Skills are **plain-text instructions** (`SKILL.md` + `references/`). Zero dependencies, no API keys — they run on your agent's existing session quota.

---

## 📮 联系 / Contact

| | |
|---|---|
| 🎬 **抖音 / Douyin** | [https://v.douyin.com/07EjIDGVErY/](https://v.douyin.com/07EjIDGVErY/) |
| 📮 **商务合作 / Business** | **wow.vip@foxmail.com** |
| 🐙 **GitHub** | [https://github.com/yzsp-ai](https://github.com/yzsp-ai) |
| 💖 **打赏 / Support** | [afdian.com/a/yzsp-ai](https://afdian.com/a/yzsp-ai) |

## 📄 License

[MIT](LICENSE) · © 2026 [yzsp-ai](https://github.com/yzsp-ai)
