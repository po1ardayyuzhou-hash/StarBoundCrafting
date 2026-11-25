# Starbound 百科

StarBound（星界边境）1.4.4 的**离线网页图鉴**：本体 + 12 个模组（Frackin' Universe、Arcana、Voided、K'Rakoth、酿造学等）的物品、配方、星球矿产、船员与怪物,支持中文 / 拼音 / ID 搜索。

👉 [在线版](https://po1ardayyuzhou-hash.github.io/StarBoundCrafting/)　·　离线用：整个仓库拷走，双击 `index.html`

## 收录

| 项目 | 数量 | 项目 | 数量 |
|---|---|---|---|
| 物品 / 配方 | 19790 / 17234 | 星球类型 | 127 |
| 中文名 / 描述覆盖 | 99.1% / 98.7% | 怪物 | 1171 |
| 制作站 | 193 类 | 商人 / 商品 | 57 个 / 2235 条 |
| 状态效果 | 1096 | 防护背包 / 模块 | 228 |
| 船员角色 | 109 组 | 轨道目标 | 27 类 |

## 功能

- **搜索**：中文名、全拼、首字母、英文 ID 都行（`铁锭` / `tiekuang` / `tk` / `ironbar`）
- **物品与配方**：点材料看配方，点产物看获取途径（掉落 / 商人 / 宝箱 / 任务 / 挖矿）
- **星球百科**：威胁等级、天气、地心形态、群系方块，以及液体 / 空气冷凝产物；矿产按**游戏地形分层**（地表 → 浅层地下 → 地下 Ⅰ/Ⅱ/Ⅲ → 地心 → 小行星带 → 大气层）做成层选框，选中哪层就只列该层的矿物，各层权重单独标注，并给出该层的**深度区间**（按世界尺寸档 2000/3000/4000… 换算，可切换）
- **群系图鉴**：625 个群系（本体 103 + FU 288 + Arcana / Voided / K'Rakoth 等），按地表 / 地下 / 太空 / 地心 / 大气分层，列出主方块、次方块与出现在多少种星球类型上；**群系名与方块名全部中文**（叠加各汉化包补丁，材质类方块另做名称解析）
- **FU 生产**：筛粉 / 粉碎 / 离心机 / 气体离心机 / 萃取 / 冶炼六类，多产物标出**实际概率**（含无产出率）
- **其他图鉴**：酿造学、商人、船员、防护背包、怪物、状态效果、轨道目标
- **体验**：五组多选筛选（条件写入地址栏可分享）、深浅主题、`/` 聚焦搜索、手机适配

## 说明

静态快照，对应生成时的游戏版本与模组列表；不含任务奖励等动态内容。枚举值（`category`、`rarity`）刻意保留英文，以免破坏筛选逻辑。

## 配套：汉化补译 mod

补译 Arcana / Voyage / 泰坦重工 / FU 等模组里官方汉化未覆盖的文本，共 **5928 个 `.patch` + 99 个界面 `.lua`、约 1.44 万条**，另含 More Planet Info 座舱面板与导航台的两处体验修正。

> ⚠️ 文本由 **AI 生成**；叠加近 6000 个补丁会让**启动慢 1–2 分钟**（只影响启动）。介意请勿使用。

| 文件 | 内容 | 启动开销 |
|---|---|---|
| [`TranslationSupplement_Lua.pak`](TranslationSupplement_Lua.pak) | 99 个界面脚本 | 几乎为零 |
| [`TranslationSupplement_Patch.pak`](TranslationSupplement_Patch.pak) | 5928 个文本补丁 | +1–2 分钟 |

两个包互不重叠，可只装其一；整个文件放进 `Starbound/mods/`，不要解压，也不要同时保留同名目录。

### 适配整合包

与 [36 项整合合集](https://steamcommunity.com/sharedfiles/filedetails/?id=3756895383)（FU + Arcana + Voyage + 泰坦重工 + K'Rakoth + Voided + LostBound + 酿造学 + 远征等，自带 11 个简中补丁）**互补使用**：

- 合集里的简中补丁负责主体汉化，本补译补的是它们的漏译（物品 / 方块 / 任务 / 界面脚本）；`zzz_` 前缀 + 19998 优先级保证最后应用，内容只有文本字段 `replace`，与合集内全部 mod 无机制冲突，直接丢进 `mods/` 即可。
- **防重复**：合集内也打包了工坊版的[本体汉化](https://steamcommunity.com/sharedfiles/filedetails/?id=807695810)、[Fu sChinese](https://steamcommunity.com/sharedfiles/filedetails/?id=754350883)与[中文字体](https://steamcommunity.com/sharedfiles/filedetails/?id=731236006)。若走工坊订阅，请移走本地的 `SChinese/`、`FuSchinese/`、`StarCore.pak`——同一汉化装两份会让补丁重复叠加。
- 合集里的 More Planet Info 是 2019 旧版（页面自述不保证兼容 1.4.X），本补译恰好附带它的座舱面板与导航台两处显示修正，建议配套使用。
- 合集内的 More threads / Starbound Optimizer 属安慰剂类（见 [FU 官方 Performance 页](http://frackinuniverse.miraheze.org/wiki/Performance)），可自行取舍；Quest Manager Optimizer (FU) 真实有效，建议保留。
- 远征（The Last Expedition）与酿造学（Brewology）的汉化由合集自带补丁负责，本补译未覆盖这两个 mod。

## 版权

**Starbound** © Chucklefish Ltd.，本仓库仅含解析数据，不含游戏本体。中文文本来自 **SChinese**（星核汉化组，CC BY-NC-SA 4.0）、**Fu Schinese**（ProjectSky），以及 Steam 创意工坊的「克拉寇斯简中补丁」「Voided 简中补丁」「王国守卫附属汉化」。图标为游戏素材，版权归原权利人。仅供学习交流，禁止商用。
