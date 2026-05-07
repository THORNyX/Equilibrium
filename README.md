# Equilibrium

让每个玩家都能拥有宝箱的《雨中冒险2》模组。 在神器界面启用 **均衡神器（Artifact of Equilibrium）** 即可生效。

## 使用说明

- **该模组需要在客户端和主机上都安装才能正常运行。**

- **与我的另一个Mod[ShareChest](https://thunderstore.io/package/Muskmelovon/ShareChest/) [*src*](https://github.com/THORNyX/ShareChest/)冲突！不能同时安装两个Mod**

## 影响游戏平衡

- 游戏前期会显著增加队伍物品掉落数量，可能影响游戏平衡，但是关底BOSS会嘿嘿嘿(其实是BUG)。

## 兼容性

- 兼容性未知，问题提交至 GitHub ：https://github.com/THORNyX/Equilibrium/issues

## 安装方法

#### **模组管理器（推荐）：**[r2modman](https://thunderstore.io/package/ebkr/r2modman/) 搜索`Equilibrium`它会自动下载所需的依赖项。

#### **手动的：**

1. 将 `Equilibrium` 文件夹放入 `Risk of Rain 2\BepInEx/plugins/` 文件夹。

2. 安装依赖项：
   - BepInExPack
   - HookGenPatcher
   - RoR2BepInExPack
   - R2API.Core、R2API.ContentManagement、R2API.Language、R2API.ArtifactCode、R2API.CommandHelper、R2API.Networking

3. 启动一次游戏，配置文件:`BepInEx/config/com.Muskmelovon.equilibrium.cfg`自动生成。

## 配置说明

- `InstanceObject`生成多个该物体的副本宝箱，每个玩家一个，每个宝箱只能由其归属的玩家打开，但是掉落物可以被任何玩家拾取。
- `InstanceBoth`生成多个该物体的副本宝箱，每个玩家一个，每个宝箱只能由其归属的玩家打开，掉落物只能由其归属的玩家拾取。

| 配置项/Config | 默认值/Default | 说明/Explanation                                             |
| :------------ | :------------- | ------------------------------------------------------------ |
| `AGeneral`    | `true`         | Global master switch for Equilibrium. When false, all object instancing modes behave as None.<br />均衡神器的全局控制开关。当该开关为“false”时，所有对象实例化模式都将等同于“None”模式。（该开关由大厅内均衡神器控制，保持默认即可） |
| `ARollDrop`   | `true`         | When true, each chest copy will get a separate random seed and re-roll its items (random loot per player). When false, all copies will have the exact same items as the original chest.<br />启用独立随机掉落：每个副本宝箱将使用独立的随机种子并重新生成物品（每个玩家看到不同的掉落）。关闭时“false”，所有副本宝箱将与原宝箱掉落完全相同的物品。<br/> |
| `Chests`      | `InstanceBoth` | Default mode for all chests. InstanceObject = each player gets a copy, items free-for-all. InstanceBoth = each player gets a copy, items owner-only.<br />所有宝箱的默认模式。InstanceObject模式：任何玩家都可以拾取；InstanceBoth模式：仅自己可拾取<br/>## 以下是宝箱对应名称：<br/>## - Chest1: 普通宝箱<br/>## - Chest2: 大宝箱<br/>## - GoldChest: 传奇宝箱<br/>## - Chest1StealthedVariant: 隐藏宝箱<br/>## - CategoryChestDamage: 伤害箱<br/>## - CategoryChestHealing: 治疗箱<br/>## - CategoryChestUtility: 辅助箱<br/>## - CategoryChest2Damage: 大伤害箱<br/>## - CategoryChest2Healing: 大治疗箱<br/>## - CategoryChest2Utility: 大辅助箱<br/>## - EquipmentBarrel: 装备箱<br/>## - LunarChest: 月球舱<br/>## - VoidChest: 虚空摇篮<br/>## - Lockbox: 生锈锁箱<br/>## - ScavBackpack: 拾荒者背包 |
| `Shops`       | `InstanceBoth` | Default mode for multi shops.<br />三选一商店的默认模式<br/>## 以下是三选一商店对应名称：<br/>## - TripleShop: 三选一商店<br/>## - TripleShopLarge: 大三选一商店？<br/>## - TripleShopEquipment: 装备三选一商店<br/>## - FreeChestMultiShop: 坠毁的多功能商店maybe┑(￣Д ￣)┍ |
| `Shrines`     | `InstanceBoth` | Default mode for shrines.<br/>## 神龛的默认模式<br/>## 以下是神龛对应名称：<br/>## - ShrineChance: 机遇神龛<br/>## - ShrineBlood: 鲜血神龛<br/>## - ShrineRestack: 塑形神龛maybe |
| `Special`     | `InstanceBoth` | Default mode for sacrifice, boss drops, etc.<br/>## 牺牲、首领掉落物品等的处理方式的默认模式<br/>## 以下是牺牲、首领掉落物品对应名称：<br/>## - Sacrifice: 牺牲掉落<br/>## - HuntersTricorn: 米爹maybe<br/>## - TeleporterBoss: 传送器BOSS<br/>## - SuperRoboBallEncounter: 合金崇拜单体maybe<br/>## - BossGroup: idk┑(￣Д ￣)┍ |
| `Void`        | `InstanceBoth` | Default mode for void objects.<br/>## 虚空物品的默认模式<br/>## 以下是虚空物品对应名称：<br/>## - VoidTriple: 虚空潜能<br/>## - LockboxVoid: 结壳宝箱 |

## 待办事项

-  聊天框指令(待定)
- 多重商店修复(待定)

## 有任何问题/建议或想做出贡献？

- 请将问题或建议提交至 GitHub 代码库[：https://github.com/THORNyX/Equilibrium/issues](https://github.com/THORNyX/Equilibrium/issues)
- 小黑盒ID：19245752
- 哔哩哔哩：https://space.bilibili.com/54236953视频介绍(没做)

## 鸣谢/see also

[InstancedLoot continuation](https://thunderstore.io/package/Nicebowl/InstancedLoot_continuation/) <sup>[*src*](https://github.com/Frenqy/InstancedLoot_continuation)</sup> by [Nicebowl](https://thunderstore.io/package/Nicebowl/)

## 更新日志

- v2.0.0: 正式发布。
- v2.0.1: 修正了 `README.md` 文件中的文本格式问题
- v2.0.2: 修正了 `README.md` 文件中的文本格式问题
- v2.0.3
  - 新增 控制台命令 equilibrium_reload_config，无需重启游戏即可热重载配置。
  - 新增 控制台命令 playerlist，输入即可查看当前房间玩家列表。
  - 新增 PlayerManager，实时追踪玩家加入、离开及场景切换。
  - 新增 调试快捷键：F5 输出实时玩家列表信息，F6 强制刷新玩家数量。
  - 修复 神器名称在所有语言下统一显示为 Artifact of Equilibrium - 均衡神器。

