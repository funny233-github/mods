# Minecraft Fabric Mod 说明文档
该文档为Minecraft Fabric Mod的说明文档，涵盖模组之间的关系、依赖以及用途等信息。
## 模组列表
- [x] [iris](https://modrinth.com/mod/iris)
    - 光影
    - 优化
- [x] [starlight](https://modrinth.com/mod/starlight)
    - 光线算法优化
    - 优化
- [x] [sodium](https://modrinth.com/mod/sodium)
    - 游戏主要渲染算法优化
    - 优化
- [ ] [DistantHorizons](https://modrinth.com/mod/distanthorizons)
    - 超远视距,与iris开光影时冲突
    - 优化
- [x] [Entity Culling](https://modrinth.com/mod/entityculling)
    - 实体渲染优化
- [x] [tweakeroo](https://www.curseforge.com/minecraft/mc-mods/tweakeroo)
    - 挂
- [x] [litematica](https://www.curseforge.com/minecraft/mc-mods/litematica)
    - 投影
- [x] [itemscroller](https://www.curseforge.com/minecraft/mc-mods/item-scroller)
    - 鼠标滚轮...
- [x] [minihud](https://www.curseforge.com/minecraft/mc-mods/minihud)
    - 类f3模组
- [x] [viafabricplus](https://modrinth.com/mod/viafabricplus)
    - 跨版本进服
- [x] [firstperson](https://modrinth.com/mod/first-person-model)
    - 更好的第一人称
- [x] [notenoughanimations](https://modrinth.com/mod/not-enough-animations)
    - 更多的动画
    - 更好的第一人称附加
- [x] [emi](https://modrinth.com/mod/emi)
    - 合成配方以及更多
- [x] [emi-loot](https://modrinth.com/mod/emi-loot)
- [x] [emitrades](https://modrinth.com/mod/emitrades)
- [x] [pistorder](https://modrinth.com/mod/pistorder)
    - 方便显示活塞更新顺序
- [x] [clientcommands](https://modrinth.com/mod/client-commands)
    - 客户端命令
- [x] [carpet](https://github.com/gnembon/fabric-carpet)
- [x] [carpet-extra](https://github.com/gnembon/carpet-extra)
- [x] [XaerosWorldMap](https://modrinth.com/mod/xaeros-world-map)
    - 大地图
- [x] [XaerosMiniMap](https://modrinth.com/mod/xaeros-minimap)
    - 小地图
- [x] [very many players](https://modrinth.com/mod/vmp-fabric)
    - 优化
- [x] [chesttracker](https://modrinth.com/mod/chest-tracker)
    - 查找容纳对应物品的箱子
- [ ] [seedcrackerX](https://github.com/19MisterX98/SeedcrackerX)
    - 种子破解
- [x] [XaeroPlus](https://modrinth.com/mod/xaeroplus)
    -地图加强
- [x] [PresenceFootsteps](https://modrinth.com/mod/presence-footsteps)
- [x] [ferritecore](https://modrinth.com/mod/ferrite-core)
    - 优化
- [x] [easiervillagertrading](https://modrinth.com/mod/easiervillagertrading)
- [x] [MasaGadget](https://modrinth.com/mod/masa-gadget)
- [x] [tweakermore](https://modrinth.com/mod/tweakermore)
- [x] [OMMC][https://modrinth.com/mod/oh-my-minecraft-client]
- [x] [ItemPhysicLite](https://modrinth.com/mod/itemphysic-lite/)
- [x] [reden is what we made](https://github.com/zly2006/reden-is-what-we-made)
- [x] [inventorytabs](https://modrinth.com/mod/inventory-tabs-updated)
- [x] [itemswapper](https://modrinth.com/plugin/itemswapper)
- [x] [jsmacros](https://www.curseforge.com/minecraft/mc-mods/jsmacros)
- [x] [librarian trade finder](https://modrinth.com/mod/librarian-trade-finder)
## 主要依赖列表
- [x] [fabric-api](https://modrinth.com/mod/fabric-api)
    - 必要api
- [x] [malilib](https://www.curseforge.com/minecraft/mc-mods/malilib)
    - masa全家桶必要api
- [x] [kotlin](https://modrinth.com/mod/fabric-language-kotlin)
- [x] [modmenu](https://modrinth.com/mod/modmenu)
- [x] [cloth-config](https://modrinth.com/mod/cloth-config)
- [x] [magiclib](https://modrinth.com/mod/magiclib)
- [x] [CreativeCore](https://modrinth.com/mod/creativecore)
- [x] [syncmatica](https://modrinth.com/mod/syncmatica)
## 模组间关系图
以下是模组之间的依赖与冲突关系图，它们显示了各个模组的相互关系和依赖:
```
graph TB
iris --> sodium
DistantHorizons -.当开启光影时冲突.-> iris
tweakeroo --> malilib
litematica --> malilib
itemscroller --> malilib
minihud --> malilib
notenoughanimations --> firstperson
carpet-extra --> carpet
libIPN --> kotlin
chesttracker --> cloth-config
emi-loot --> emi
emitrades --> emi
XaeroPlus --> XaerosMiniMap
XaeroPlus --> XaerosWorldMap
XaeroPlus --> fabric-api
MasaGadget --> magiclib
tweakermore --> magiclib
emi-loot --> emi
itemswapper --> fabric-api
inventorytabs --> fabric-api
inventorytabs --> modmenu
```
