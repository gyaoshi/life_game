# itch.io 商店页文字素材 · Store Page Copy

> 说明：本文件按 itch.io「Edit game → 基本信息 + 描述」的字段顺序编排。
> 英文版在前（itch.io 默认展示语言），中文版在后，可直接复制粘贴。
> 标有 `【字段名】` 的行对应 itch.io 后台的具体输入框。

---

# 🇬🇧 ENGLISH

## 【Title】
**100 Seconds · A Life**

## 【Short description / tagline】(one line, shows on the cover tile)
You have 100 seconds to live an entire life. How much of it will you actually get done?

## 【Full description】

### One hundred seconds. One whole life.

A tiny pixel figure falls out of the sky, gets up, and starts walking right. From that first breath to the last, **48 "things everyone is supposed to do"** come flying at you one after another — and the clock never stops.

How many you manage to finish is the completion rate of your life.

It takes 100 seconds. It feels like a lot longer. When your figure finally reaches the tombstone, you may find yourself asking the question the game is really about: **out of everything you rushed through, what actually mattered?**

---

### How it plays

Five kinds of interaction rotate through the whole life, and the windows get tighter as you go (from ~5 seconds down to ~3):

| Action | What you do |
|---|---|
| **Tap** | Click a moving object out of the air |
| **Rapid tap** | Mash fast enough within the window |
| **Hold** | Press and hold until the bar fills |
| **Drag** | Drag an object into the dashed box |
| **Choose** | Pick the "socially correct" answer out of three |

The 48 events span eight stages of life — **Birth · Childhood · Teens · Youth · Prime · Middle Age · Old Age · Twilight**:

drinking your first milk, the first-birthday grab test, homework, morning radio exercises, the college entrance exam, sending out résumés, the job interview, pulling an all-nighter, saving for a down payment, buying a home, getting married, holding your newborn, paying off the mortgage, helping with homework, business dinners and toasts, the annual physical, saying goodbye to your parents, retirement, square dancing in the park, taking your pills on time, watching one sunset, calling your kids…

**The ending.** Your figure stops at the tombstone. Eight cards float in front of you — **the one you loved, your children, your parents, your career, money, freedom, the sunsets you saw, the words you never said.** You may take **only one**. The rest scatter on the spot. The one you keep is carved into the headstone.

Then you get graded in **8 tiers**, from *Winner at life* all the way down to *A walking husk*.

---

### Features

- **The whole life in 100 seconds** — 48 scripted events, one per beat, escalating pressure.
- **Full localization: English · 中文 · 日本語 · Русский.** Switch languages any time from the menu or the results screen. The game auto-detects your browser language on first launch.
- **96 bespoke success/failure animations** — every single one of the 48 events has its own pair of outcomes. Get the vaccine and an immunity shield rises from your feet; miss it and a swarm of viruses rains down. Shoulder the backpack and the straps tighten; miss it and the bag hits the ground and books scatter everywhere.
- **Objects you drop stay behind.** Nothing pops out of existence. Whatever falls out of your hands settles on the ground and slowly drifts backward with the scenery — the task walks on, but the past stays in the past.
- **Companions walk with you — then stay behind.** In 22 of the 48 events, succeeding means **someone walks beside you for 5 seconds** — a girlfriend, a bride, your parents, a child, a friend, a dog. They queue up shoulder to shoulder so nobody ever overlaps. And when their five seconds are up they don't blink out of existence: they stop, stay where they are, and drift back into the distance while you walk on. A love interest makes way for the bride; the bride makes way for the child.
- **Everything is generated in code.** Every sprite, every note, every grunt is synthesized at runtime. There is not a single asset file in the build.
- **Single file, zero dependencies.** One HTML file. No install, no download size, no network. Open it in a browser and play.

---

### Controls

- **Mouse** — click, hold, and drag.
- **Touch** — fully playable on phones and tablets (works great in a mobile browser or as a fullscreen page).
- The canvas auto-scales to your window, always at a crisp integer pixel ratio.

> Sound starts after your first click (browsers require a user gesture before audio).

---

### Technical notes (for the curious)

- **Pixel rendering:** a 480×270 internal canvas, upscaled by an integer factor with `imageSmoothingEnabled = false` to preserve hard pixel edges. Chinese/Japanese/Russian text is drawn on the *main* canvas at logical coordinates, so crisp type and chunky pixels coexist.
- **Art:** 32 hand-authored 8×8 character-map icons and a fixed palette; one primitive (`wpx`) draws everything.
- **Scenery:** 8 themes (pink delivery room → blue-sky childhood → grey middle age → orange sunset → purple twilight), banded sky gradients, parallax clouds, and alternating city skylines and rolling hills.
- **Music:** a real-time 8-bit sequencer built on the Web Audio API — 32 steps, an Am–F–C–G progression, pentatonic arpeggios, noise hats. **The tempo climbs from 148 to 218 BPM** as life speeds up. The character speaks in a synthesized `gibberish()` mumble.
- **Timeline:** per-event real ages act as control points for a piecewise-linear `ageAt(t)`; age, scenery stage and event stay locked together, and time accelerates as you age.
- **Hero animation:** a single-slot state machine drives a five-axis pose (offset / scale / tilt / arms / expression). 12 generic actions + 8 `heroAura` overlays (immunity shield, sickness, sleepiness, anger, sweat, heartbreak, coins, muscle), and world scroll drops to 32% during an action for a deliberate "beat of pause."

---

### Content notes

Themes of mortality, aging and loss; a mild, non-graphic depiction of a character's death (they reach a tombstone). Pixel-art blood is not depicted. Suitable for all ages.

---

## 【Genre】
`Simulation` (or `Action`)

## 【Tags】(pick up to 10 — suggested, in priority order)
`pixel-art`, `reaction`, `clicker`, `life-simulation`, `short`, `2d`, `chiptune`, `singleplayer`, `narrative`, `experimental`

## 【Made with】
`HTML5`, `JavaScript`

## 【Languages supported】(itch.io language checkboxes)
- English ✔
- Chinese (Simplified) ✔
- Japanese ✔
- Russian ✔

## 【Price】
Free — **or** "Name your own price" (suggested: $0 with an optional tip). It's a self-contained, single-file experience; pay-what-you-want fits a 100-second game well.

## 【Screenshots】(ready to upload from `dist/`, 1440×810)

| File | Caption |
|---|---|
| `dist/shot-1-menu.png` | 100 seconds. One life. Pick your language and begin. |
| `dist/shot-2-play.png` | Tap, mash, hold, drag, choose — the windows keep closing. |
| `dist/shot-3-mates.png` | Get it right and someone walks beside you. |
| `dist/shot-9-companions.png` | Companions queue up — they never overlap. |
| `dist/shot-4-debris.png` | Drop something? It stays on the ground and drifts into the past. |
| `dist/shot-5-final.png` | Eight cards. You may take only one. |
| `dist/shot-6-result.png` | Then you're graded — from "Winner at life" to "A walking husk." |
| `dist/shot-7-ja.png` | 日本語対応 — full Japanese localization. |
| `dist/shot-8-ru.png` | Полная русская локализация — and 中文 too. |

> The game runs at a 480×270 pixel canvas and is always displayed at an integer
> upscale, so screenshots come out crisp at any size. 1440×810 = exactly 3×.

---
---

# 🇨🇳 中文版

## 【标题】
**一生 · 100 秒**

## 【短描述 / 一句话简介】（封面卡片上显示）
用 100 秒过完一辈子。你到底来得及做完多少？

## 【完整描述】

### 一百秒，一辈子。

一个像素小人从天而降，爬起来，开始往右走。从第一口奶到最后一口药，**48 件「这辈子该做的事」**劈头盖脸一件接一件砸过来——而钟一直在走。

你来得及做完多少，就是你这一生的完成度。

它只需要 100 秒。却让人觉得过了很久很久。当小人终于走到墓碑前，你大概会忍不住问出这个游戏真正想问的那句话：**忙忙碌碌赶完的这一切里，到底哪一样才是重要的？**

---

### 怎么玩

五种交互轮着来，越到后面窗口越挤（从约 5 秒压到约 3 秒）：

| 交互 | 你要做的事 |
|---|---|
| **点** | 点掉正在横向移动的物体 |
| **连点** | 在窗口内快速点够次数 |
| **按住** | 按住不放，撑到进度条满 |
| **拖拽** | 把物体拖进虚线方框 |
| **选择** | 从三个选项里挑「社会标准答案」 |

48 件事覆盖人生八个阶段——**出生 · 童年 · 少年 · 青年 · 而立 · 中年 · 老年 · 暮年**：

喝第一口奶、抓周、写作业、广播体操、高考、投简历、面试、通宵加班、攒首付、买房、结婚、抱起新生儿、还房贷、辅导作业、应酬敬酒、体检报告、送别父母、办退休、跳广场舞、按时吃药、看一次夕阳、给儿女打个电话……

**结尾。** 小人停在墓碑前，8 张卡片漂在面前——**爱人、孩子、父母、事业、钱、自由、看过的夕阳、没说出口的话。** 你**只能带走一样**，其余当场散掉，那一样刻在墓碑上。

最后按完成率给你 8 档评价，从「人生赢家」一路到「一具行走的躯壳」。

---

### 特色

- **100 秒过完一生** —— 48 个剧情事件，一格接一格，压力层层加码。
- **完整多语言：English · 中文 · 日本語 · Русский。** 在开始界面或结算界面随时切换；首次进入时会按浏览器语言自动选择。
- **96 套专属成功/失败动画** —— 48 件事，每一件都配了**自己的**一对演出。打疫苗成功，蓝色免疫护盾从脚下升起；失败，病毒成群落下来。背书包成功，肩带收紧；失败，书包砸在地上、书本四散。
- **掉在地上的东西不会消失。** 没有任何东西凭空蒸发——从手里掉出去的东西会落在地上，跟着背景慢慢后移。任务往前走了，过去留在过去。
- **有人陪你走，然后留在原地。** 48 件事里有 22 件，成功后**会有人陪着你走 5 秒**——恋人、新娘、父母、孩子、朋友、狗。他们会自动排队并肩走，绝不前后重叠；五秒一到也不会凭空消失，而是停下来停在原处，随着你继续往前走，慢慢退到身后。恋人出现会让上一任让位；新娘一上场，恋人先退场；孩子出生，新娘退场。
- **所有东西都由代码实时生成。** 每一帧画面、每一个音符、每一声含糊的人声都是运行时算出来的——打包里没有任何一个素材文件。
- **单文件、零依赖。** 就一个 HTML 文件。不用装、不用下、不用联网，浏览器里打开就是游戏。

---

### 操作

- **鼠标** —— 点击、按住、拖拽。
- **触屏** —— 手机、平板上完整可玩（移动端浏览器或全屏页面体验最佳）。
- 画布会自适应窗口大小，始终保持整数倍缩放，像素不会被拉糊。

> 首次点击画面后才会出声（浏览器要求用户手势才能启动音频）。

---

### 技术细节（给好奇的人）

- **像素渲染**：480×270 的内部分辨率，整数倍放大到主画布，`imageSmoothingEnabled = false` 保住硬像素边缘。中/日/俄文文字画在**主画布**的逻辑坐标上，所以清晰的字体和粗颗粒的像素可以共存。
- **美术**：32 个手写 8×8 字符画图标 + 固定调色板；所有绘制都走同一个原语（`wpx`）。
- **场景**：8 个主题（粉色产房 → 蓝天童年 → 灰色中年 → 橙色夕阳 → 紫色暮年），天空分带渐变、视差云层，城市天际线与圆弧山丘交替。
- **音乐**：基于 Web Audio 的实时 8bit 音序器——32 步、Am–F–C–G 和声进行、五声音阶琶音、噪声踩镲。**BPM 从 148 一路飙到 218**，人生越走越急。小人开口是 `gibberish()` 合成的含糊人声。
- **时间轴**：以每个事件的真实年龄为控制点做分段线性插值 `ageAt(t)`，年龄、场景阶段、事件三者严格对齐，越老时间过得越快。
- **小人动画**：单槽状态机驱动五组姿态（位移 / 缩放 / 倾斜 / 手臂 / 表情），12 种通用动作 + 8 种 `heroAura` 挂件（免疫护盾、病气、睡意、怒气、汗、心碎、金币、肌肉），做动作时世界滚动降到 32%，形成「停顿一拍」的节奏。

---

### 内容提示

涉及死亡、衰老与失去的主题；对角色死亡的处理很温和、不写实（走到一块墓碑前）。没有血腥描写。适合所有年龄。

---

## 【分类 Genre】
`Simulation`（或 `Action`）

## 【标签 Tags】（最多选 10 个，已按优先级排序）
`pixel-art`、`reaction`、`clicker`、`life-simulation`、`short`、`2d`、`chiptune`、`singleplayer`、`narrative`、`experimental`

## 【Made with】
`HTML5`、`JavaScript`

## 【支持语言】（itch.io 语言勾选项）
- English ✔
- Chinese (Simplified) ✔ 简体中文
- Japanese ✔ 日本語
- Russian ✔ Русский

## 【价格】
免费 —— 或选择「Name your own price」（建议 $0 + 可选打赏）。它是一段自成体系、单文件、随时能玩完的体验，随缘付费很适合一个 100 秒的游戏。

## 【截图】（现成的，在 `dist/` 里，1440×810）

| 文件 | 配文 |
|---|---|
| `dist/shot-1-menu.png` | 100 秒，一辈子。选好语言就开始。 |
| `dist/shot-2-play.png` | 点、连点、按住、拖拽、选择——窗口一个比一个急。 |
| `dist/shot-3-mates.png` | 做对了，会有人陪你一起走。 |
| `dist/shot-9-companions.png` | 同伴会自动排队并肩走，绝不前后重叠。 |
| `dist/shot-4-debris.png` | 掉在地上的东西不会消失，它跟着背景慢慢退向过去。 |
| `dist/shot-5-final.png` | 八张卡片。你只能带走一样。 |
| `dist/shot-6-result.png` | 然后你被评分——从「人生赢家」到「一具行走的躯壳」。 |
| `dist/shot-7-ja.png` | 日本語対応——完整日语本地化。 |
| `dist/shot-8-ru.png` | Полная русская локализация——当然还有中文。 |

> 游戏内部是 480×270 的像素画布，永远按整数倍放大显示，所以任何尺寸截图都清晰。
> 1440×810 正好是 3 倍。

---
---

# 附：一句话社媒文案 / Social one-liners

**EN**
- 100 seconds. 48 things to do. One life to spend. How much of it will you get done?
- A pixel-art game about how fast a life goes by — and what you'd keep.

**中文**
- 100 秒过完一辈子，48 件事劈头盖脸砸过来。你来得及做完多少？
- 一个像素小人，一百秒，一辈子。走到墓碑前，你只能带走一样东西。

---

# 附：上传清单 / Upload checklist

上传时 itch.io 后台还需要这几项，留意一下：

| 项目 | 说明 |
|---|---|
| **Cover image** | **必填**，建议 630×500（≥315×250）。目前仓库里还没有，可以用 `dist/shot-5-final.png` 或 `shot-2-play.png` 临时顶替，也可以单独做一张标题卡。 |
| **Screenshots** | `dist/shot-1..9*.png`，9 张 1440×810，直接拖进上传框。 |
| **Kind of project** | `HTML` （itch.io 会直接托管、在浏览器里跑）。 |
| **Uploads** | 把 `life-game.html` **改名成 `index.html`** 再压缩成 zip 上传——itch.io 默认只认 zip 根目录下的 `index.html`。 |
| **Viewport / Embed** | 建议勾选 `Mobile friendly` 并让画面自适应；游戏本身已经处理了触摸与缩放。 |
| **Pricing** | Free 或 Name your own price。 |
| **Languages** | English / Chinese (Simplified) / Japanese / Russian。 |

> 单文件、零依赖，所以 zip 里只有 `index.html` 一个文件就够，体积很小。
