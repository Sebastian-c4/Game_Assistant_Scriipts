[简体中文](README.md) | [English](README-EN.md)

# 瓦斯辅助脚本

**作者：c4_angel**  
**支持语言：简体中文，英文**  
**版本：1.6**  [更新历史](CHANGELOG.md)

## 兼容性及安装说明
- 本模组支持版本2.5或以上的博德之门增强版（BGEE）、龙矛围攻（SOD）、博德之门2增强版（BG2EE），以及增强版三部曲（EET）
- 在龙矛围攻（SOD）上安装时须先使用 Modmerge 或 DLC Merger。[DLC Merger下载地址](https://github.com/Argent77/A7-DlcMerger/releases/latest)
- 基于脚本的判断需求，本脚本会对游戏内大量法术文件进行无实际效果的处理，为保证脚本正常运行，**必须**在所有引入新法术/技能，或是对后缀为.SPL的文件进行覆盖型修改的模组**之后**安装，最典型的如法术修订（SR）。
- 本模组占用至少2条SPLSTATE.ids文件的空白条目（视模组安装环境还可能占用更多）。如当前游戏环境下无足够空余空间可能导致本脚本安装失败。
- 在脚本安装开始时会提示玩家设置热键，一共三个。三个热键为脚本完整工作所必需。你也可以使用预置的ini文件进行设置，或是在任何时候使用组件二调整热键设置。

## 内容介绍
本模组旨在使那些无聊、机械重复又浪费时间的很多操作通过游戏脚本自动完成。  
模组目前主要有三大功能：战斗脚本、自动暂停和一键Buff系统。  
使用方式：
- 开启系统AI（游戏默认热键A，或点击画面右下角的锁型图标切换开启或关闭）
- 在游戏内选定人物
- 按下所设置的控制台热键
- 进行你想要的设置

**注意：除自动暂停外，脚本其他两大功能均必须在开启了系统AI之后才能正常工作。**

### 战斗脚本
如同其他AI脚本一样，此脚本控制无指令状态下人物的行为。
- 遇敌自动攻击：可设置三种模式：攻击武器范围内的最近敌人（默认）；主动上前攻击视野内的最近敌人；不进行主动攻击
- 隐身时攻击状态：不主动攻击（默认）；以上述设定的模式决定攻击行为
- 在开启侦测陷阱/超渡时：不主动攻击（默认）；以上述设定的模式决定攻击行为
- 吟游诗人自动吟唱（默认）；不自动吟唱（例如无歌曲效果的舞剑士）
- 盗贼/潜行者在周围无敌人时自动潜行（默认）；不自动潜行

### 自动暂停
当物理防护法术失效时自动暂停游戏，包括两类。此功能为全局设定，默认禁用。
- 石肤术、铁皮术（人物须为法师、德鲁伊、牧师/游侠，或掌握万能巧手能力）
- 防护魔法武器、壁罩术系列（人物须为法师，或掌握万能巧手能力）
	
### 一键Buff系统
使用一键Buff需要满足两个条件：
- AI模式开启
- 非战斗状态，所有队员身边没有敌人
在满足条件时按下自身或团队Buff热键即可启动Buff进程。更多详细说明见控制台。

支持的法术类型包括：
- 奥术：例如石肤术（仅自身）、幸运术（自身、团队）、高等加速术（仅团队）
- 神术：例如信仰铠甲（仅自身）、防死结界（自身、团队）、巨力术（仅团队）
- 天赋技能（默认不自动施放）：例如强韧（仅自身）
- 延迟施放类（避免阻挡队友的增益法术，延迟一轮施放）：例如法术无效结界（仅自身）
- 抗性增强奥术（同时包含自身和团队）：例如防护强酸
- 抗性增强神术（同时包含自身和团队）：例如抵抗火焰和寒冷
	
**注意：本功能目前可识别纯增强版、“强化铁砧v6.4”、“永恒原力v4.4”、“QC宗派集合”所包含的法术，所支持法术会因当前游戏环境的不同而有所差别。请以游戏内控制台中所列法术为准。**

