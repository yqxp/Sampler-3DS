# Sampler-3DS
This is a (not really) simple 3DS sampler. Multisample supported. 

Up to **8 zones** — a zone is a key range, a sample and a full set of patch parameters — so for example, a kick, a bass, a guitar and a lead can live in one pattern (yes there is piano roll too). 

## Features

| | |
|---|---|
| **Engine** | 8 voices, 16-bit fixed point, 32728.5 Hz mono out (NDSP) |
| **Sound Sources** | triangle, saw, **W1–W4** (`16-bit mono PCM` WAVs you put on the card), microphone |
| **Filter on each voice** | SVF with `CLEAN` and `ACID` voicings, cut / Q / gain / accent / ENV AMT (ADV panel) |
| **FX chain** | DIST · LIMITER · REVERB · IMAGER · CHORUS · ECHO |
| **Pattern (Piano roll)** | 16 steps per bar, 1 / 2 / 4 / 8 bars, copy / paste, 8-step undo |
| **3D Topscreen** | layered depth on the top screen; 3D extended banner in the HOME menu |
| **Save Your Projects** | `.pat` files on the SD card — save / load / rename / delete |

## Install

You need a **3DS / 2DS with custom firmware** (Luma3DS) and **FBI**, or a 3DS emulator such as
Azahar.

1. Download `sampler-3ds-<version>.cia` from [Releases](https://github.com/yqxp/Sampler-3DS/releases).
2. Copy it anywhere on the SD card.
3. Open **FBI → SD → the file → Install**.

*On first launch the app creates*

```
sdmc:/3ds/sampler-3ds/
    samples/     *.wav   ← 16-bit mono PCM, your own material
    songs/       *.pat   ← projects
```

Drop your own `16-bit mono PCM` WAVs into `samples/` and pick them on the **FILES** page.

## Credits

- Built with **devkitPro** — `libctru`, `citro2d` / `citro3d`, `tex3ds`, `bannertool`, `makerom`.
- Tested in the **Azahar** emulator, and of course on my lovely real machine.
- Engine, UI, the 3D banner model and the factory samples — [YQXP MUSIC](https://www.youtube.com/channel/UCJMLpzIQah8ErPu-YiGw7Uw) (myself)

*Binary builds are free to install and play with on your own console. The source is not distributed.*

# Sampler-3DS（中文）

这是一个**（不太）简单**的 3DS 采样器。支持多重采样（multisample）。

最多 **8 个 zone** —— 一个 zone = 一段音区 + 一个采样 + 一整套音色参数；所以底鼓、bass、吉他、
lead 可以住在同一条 pattern 里（对的对的，甚至有钢琴卷帘窗）。

## 功能

| | |
|---|---|
| **引擎** | 8 声部、16 位定点、32728.5 Hz 单声道输出（NDSP） |
| **音源** | 三角波、锯齿波、**W1–W4**（你自己放进 SD 卡的 `16-bit 单声道 PCM` WAV）、麦克风 |
| **每个声部独立滤波器** | SVF，`CLEAN` 与 `ACID` 两种味道，cut / Q / gain / accent / ENV AMT（ADV 面板） |
| **效果链** | DIST · LIMITER · REVERB · IMAGER · CHORUS · ECHO |
| **Pattern（钢琴卷帘）** | 每小节 16 步，1 / 2 / 4 / 8 小节，复制 / 粘贴，8 步撤销 |
| **3D 上屏** | 上屏有分层景深 |
| **工程保存** | SD 卡上的 `.pat` 文件 —— 保存 / 载入 / 改名 / 删除 |

## 安装

需要**装了自制系统（Luma3DS）的 3DS** 和 **FBI**，或者 Azahar 之类的 3DS 模拟器。

1. 到 [Releases](https://github.com/yqxp/Sampler-3DS/releases) 下载 `sampler-3ds-<版本>.cia`。
2. 拷到 SD 卡里任意位置。
3. 打开 **FBI → SD → 选中那个文件 → Install**。

*第一次启动时，程序会建出：*

```
sdmc:/3ds/sampler-3ds/
    samples/     *.wav   ← 16-bit 单声道 PCM，放你自己的素材
    songs/       *.pat   ← 工程
```

把 `16-bit 单声道 PCM` 的 WAV 丢进 `samples/`，然后在 **FILES** 页里选。

## 致谢

- 用 **devkitPro** 构建 —— `libctru`、`citro2d` / `citro3d`、`tex3ds`、`bannertool`、`makerom`。
- 在 **Azahar** 模拟器里测试，当然也在我的实机上。
- 引擎、界面、3D banner 模型与出厂采样 —— [YQXP MUSIC](https://www.youtube.com/channel/UCJMLpzIQah8ErPu-YiGw7Uw)（没错，就是我）

*编译好的 CIA 可以随便装到你自己的机器上玩；源码不分发。*
