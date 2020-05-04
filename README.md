---- Minecraft Crash Report ----
// Daisy, daisy...

Time: 5/3/20 5:59 PM
Description: Updating screen events

java.lang.NoSuchMethodError: net.minecraft.item.ItemStack.getItem()Lnet/minecraft/item/Item;
	at net.mcft.copy.betterstorage.api.BetterStorageUtils.wildcardMatch(BetterStorageUtils.java:18)
	at net.mcft.copy.betterstorage.item.recipe.ComboRecipe.checkMatch(ComboRecipe.java:63)
	at net.mcft.copy.betterstorage.item.recipe.ComboRecipe.func_77569_a(ComboRecipe.java:35)
	at net.mcft.copy.betterstorage.item.recipe.KeyRecipe.func_77569_a(KeyRecipe.java:31)
	at net.minecraft.item.crafting.CraftingManager.func_82787_a(CraftingManager.java:323)
	at net.minecraft.inventory.ContainerPlayer.func_75130_a(ContainerPlayer.java:80)
	at net.minecraft.inventory.InventoryCrafting.func_70299_a(SourceFile:81)
	at net.minecraft.inventory.Slot.func_75215_d(Slot.java:77)
	at net.minecraft.inventory.Container.func_75144_a(SourceFile:222)
	at net.minecraft.client.multiplayer.PlayerControllerMP.func_78753_a(PlayerControllerMP.java:419)
	at net.minecraft.client.gui.inventory.GuiContainer.func_146984_a(GuiContainer.java:641)
	at net.minecraft.client.gui.inventory.GuiContainer.func_146286_b(GuiContainer.java:607)
	at net.minecraft.client.gui.GuiScreen.func_146274_d(GuiScreen.java:306)
	at net.minecraft.client.gui.GuiScreen.func_146269_k(GuiScreen.java:268)
	at net.minecraft.client.Minecraft.func_71407_l(Minecraft.java:1640)
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:973)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:898)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at net.mcft.copy.betterstorage.api.BetterStorageUtils.wildcardMatch(BetterStorageUtils.java:18)
	at net.mcft.copy.betterstorage.item.recipe.ComboRecipe.checkMatch(ComboRecipe.java:63)
	at net.mcft.copy.betterstorage.item.recipe.ComboRecipe.func_77569_a(ComboRecipe.java:35)
	at net.mcft.copy.betterstorage.item.recipe.KeyRecipe.func_77569_a(KeyRecipe.java:31)
	at net.minecraft.item.crafting.CraftingManager.func_82787_a(CraftingManager.java:323)
	at net.minecraft.inventory.ContainerPlayer.func_75130_a(ContainerPlayer.java:80)
	at net.minecraft.inventory.InventoryCrafting.func_70299_a(SourceFile:81)
	at net.minecraft.inventory.Slot.func_75215_d(Slot.java:77)
	at net.minecraft.inventory.Container.func_75144_a(SourceFile:222)
	at net.minecraft.client.multiplayer.PlayerControllerMP.func_78753_a(PlayerControllerMP.java:419)
	at net.minecraft.client.gui.inventory.GuiContainer.func_146984_a(GuiContainer.java:641)
	at net.minecraft.client.gui.inventory.GuiContainer.func_146286_b(GuiContainer.java:607)
	at net.minecraft.client.gui.GuiScreen.func_146274_d(GuiScreen.java:306)
	at net.minecraft.client.gui.GuiScreen.func_146269_k(GuiScreen.java:268)

-- Affected screen --
Details:
	Screen name: net.minecraft.client.gui.inventory.GuiInventory

-- Affected level --
Details:
	Level name: MpServer
	All players: 1 total; [EntityClientPlayerMP['Clossis'/9615, l='MpServer', x=24.69, y=76.62, z=-42.38]]
	Chunk stats: MultiplayerChunkCache: 418, 418
	Level seed: 0
	Level generator: ID 00 - default, ver 1. Features enabled: false
	Level generator options: 
	Level spawn location: World: (-42,64,-10), Chunk: (at 6,4,6 in -3,-1; contains blocks -48,0,-16 to -33,255,-1), Region: (-1,-1; contains chunks -32,-32 to -1,-1, blocks -512,0,-512 to -1,255,-1)
	Level time: 6325 game time, 6325 day time
	Level dimension: 0
	Level storage version: 0x00000 - Unknown?
	Level weather: Rain time: 0 (now: false), thunder time: 0 (now: false)
	Level game mode: Game mode: survival (ID 0). Hardcore: false. Cheats: false
	Forced entities: 157 total; [EntityCreeper['Creeper'/2560, l='MpServer', x=-29.50, y=80.00, z=-62.50], EntityCreeper['Creeper'/9218, l='MpServer', x=70.50, y=61.00, z=-51.69], EntityCreeper['Creeper'/9219, l='MpServer', x=69.00, y=62.00, z=-53.75], EntityClientPlayerMP['Clossis'/9615, l='MpServer', x=24.69, y=76.62, z=-42.38], EntityCreeper['Creeper'/9220, l='MpServer', x=70.50, y=61.00, z=-52.69], EntityCovenWitch['Coven Witch'/261, l='MpServer', x=79.88, y=72.38, z=-14.50], EntityArrow['arrow'/9991, l='MpServer', x=53.56, y=71.97, z=-9.63], EntityCreeper['Creeper'/8969, l='MpServer', x=37.31, y=43.00, z=-35.75], EntityItem['item.tile.sapling.spruce'/9993, l='MpServer', x=10.54, y=84.89, z=-52.88], EntityCreeper['Creeper'/8970, l='MpServer', x=38.38, y=43.00, z=-36.47], EntityZombie['Zombie'/8971, l='MpServer', x=37.34, y=43.00, z=-36.69], BlueSlime['Blue Slime'/5134, l='MpServer', x=38.66, y=43.00, z=-35.06], EntityFireworkRocket['entity.FireworksRocketEntity.name'/10003, l='MpServer', x=27.51, y=78.48, z=-45.48], EntityCreeper['Creeper'/7961, l='MpServer', x=-14.50, y=34.00, z=-9.50], EntityZombie['Zombie'/7962, l='MpServer', x=-15.50, y=34.00, z=-8.50], EntityZombie['Zombie'/9503, l='MpServer', x=43.50, y=50.00, z=-2.50], EntityCreeper['Creeper'/9504, l='MpServer', x=43.38, y=53.00, z=0.94], EntityZombie['Zombie'/9270, l='MpServer', x=40.50, y=49.00, z=-9.50], EntityBat['Bat'/9785, l='MpServer', x=-53.59, y=61.41, z=-89.00], EntityCreeper['Creeper'/9531, l='MpServer', x=31.44, y=43.00, z=-15.97], EntityCreeper['Creeper'/9020, l='MpServer', x=24.63, y=22.00, z=-45.06], EntityZombie['Zombie'/8514, l='MpServer', x=-18.50, y=20.00, z=-104.50], EntityItem['item.tile.tropicraft:flower_8'/5451, l='MpServer', x=4.69, y=83.13, z=-100.09], EntityCreeper['Creeper'/9040, l='MpServer', x=30.28, y=56.00, z=-24.13], EntitySkeleton['Skeleton'/6480, l='MpServer', x=-52.70, y=72.00, z=-71.12], EntityItem['item.item.stick'/9553, l='MpServer', x=24.72, y=75.13, z=-39.13], EntitySkeleton['Skeleton'/5969, l='MpServer', x=2.16, y=76.00, z=-53.56], EntitySkeleton['Skeleton'/5970, l='MpServer', x=11.13, y=75.00, z=-56.53], EntityItem['item.tile.flowers2.minersdelight'/6484, l='MpServer', x=33.19, y=40.13, z=-0.09], EntitySkeleton['Skeleton'/7523, l='MpServer', x=13.91, y=53.00, z=-15.44], EntityItem['item.item.seeds'/8291, l='MpServer', x=-9.88, y=83.13, z=-57.81], EntitySkeleton['Skeleton'/7781, l='MpServer', x=77.50, y=57.00, z=-34.50], EntitySkeleton['Skeleton'/7534, l='MpServer', x=45.56, y=36.00, z=-7.94], EntitySkeleton['Skeleton'/7535, l='MpServer', x=44.16, y=37.00, z=-14.50], EntityItem['item.item.sulphur'/9330, l='MpServer', x=18.16, y=22.13, z=-44.88], EntityItem['item.tile.sapling.spruce'/9331, l='MpServer', x=9.88, y=80.13, z=-53.09], EntityZombie['Zombie'/6524, l='MpServer', x=-31.50, y=23.00, z=-26.50], EntityItem['item.tile.flowers2.minersdelight'/5245, l='MpServer', x=45.88, y=11.13, z=-25.19], EntitySkeleton['Skeleton'/8830, l='MpServer', x=42.50, y=53.00, z=3.50], EntitySkeleton['Skeleton'/8835, l='MpServer', x=36.50, y=40.00, z=-2.16], EntityItem['item.tile.flowers2.minersdelight'/5252, l='MpServer', x=31.19, y=40.13, z=-1.34], EntityZombie['Zombie'/7045, l='MpServer', x=-2.50, y=20.00, z=-122.50], EntityItem['item.tile.flowers2.minersdelight'/5263, l='MpServer', x=34.19, y=40.13, z=2.53], EntityCustomMob10000['Bandit'/9873, l='MpServer', x=52.34, y=70.00, z=-8.66], EntityCustomMob10000['Bandit'/9874, l='MpServer', x=56.16, y=70.00, z=-9.31], EntityItem['item.tile.flowers2.minersdelight'/5266, l='MpServer', x=31.19, y=40.13, z=5.91], EntityItem['item.tile.gravel'/1684, l='MpServer', x=-10.47, y=85.13, z=-103.38], EntityItem['item.tile.flowers2.minersdelight'/5269, l='MpServer', x=30.19, y=40.13, z=7.19], EntityItem['item.tile.gravel'/1685, l='MpServer', x=-10.59, y=85.13, z=-104.59], EntityCow['Cow'/149, l='MpServer', x=-49.50, y=89.00, z=-21.50], EntityZombie['Zombie'/8085, l='MpServer', x=-55.53, y=82.00, z=-85.91], EntityBat['Bat'/9622, l='MpServer', x=80.53, y=29.00, z=-36.28], EntityCow['Cow'/150, l='MpServer', x=-52.69, y=86.00, z=-33.53], EntityBat['Bat'/9623, l='MpServer', x=89.00, y=35.07, z=-35.47], EntityItem['item.tile.flowers2.minersdelight'/5271, l='MpServer', x=30.19, y=40.13, z=-2.88], EntityCow['Cow'/151, l='MpServer', x=-50.78, y=89.00, z=-20.25], EntityBat['Bat'/9624, l='MpServer', x=83.16, y=34.34, z=-37.41], EntityCow['Cow'/152, l='MpServer', x=-44.59, y=82.00, z=-1.63], EntitySquid['Squid'/9625, l='MpServer', x=85.28, y=58.00, z=-34.50], EntitySheep['Sheep'/9626, l='MpServer', x=88.50, y=74.00, z=-40.35], EntitySheep['Sheep'/9627, l='MpServer', x=88.06, y=70.00, z=-34.84], EntitySpider['Spider'/9628, l='MpServer', x=96.19, y=19.00, z=-20.19], EntityItem['item.tile.flowers2.minersdelight'/5276, l='MpServer', x=32.19, y=40.13, z=-1.16], EntitySheep['Sheep'/9629, l='MpServer', x=93.50, y=70.00, z=-27.50], EntityCow['Cow'/157, l='MpServer', x=-4.06, y=92.00, z=-29.97], EntitySheep['Sheep'/9630, l='MpServer', x=87.41, y=70.00, z=-27.47], EntityBat['Bat'/6046, l='MpServer', x=22.31, y=44.24, z=-62.03], EntityVillageGuard['Guard'/9632, l='MpServer', x=58.31, y=70.00, z=-12.25], EntityVillager['Villager'/9633, l='MpServer', x=97.25, y=71.00, z=-5.75], EntitySheep['Sheep'/9634, l='MpServer', x=96.09, y=71.00, z=-9.59], EntitySheep['Sheep'/9635, l='MpServer', x=92.66, y=71.00, z=-9.47], EntityZombie['Zombie'/9379, l='MpServer', x=26.50, y=17.00, z=-45.50], EntitySheep['Sheep'/9636, l='MpServer', x=92.66, y=71.00, z=-7.84], EntityCustomMob10000['Bandit'/6564, l='MpServer', x=24.50, y=34.00, z=4.50], EntityItemFrame['entity.ItemFrame.name'/9637, l='MpServer', x=91.50, y=74.50, z=-2.94], EntityItem['item.tile.cloth.white'/933, l='MpServer', x=38.47, y=69.13, z=16.13], EntityItemFrame['entity.ItemFrame.name'/9638, l='MpServer', x=92.50, y=74.50, z=-2.94], EntityItem['item.tile.cloth.gray'/934, l='MpServer', x=48.38, y=75.13, z=-19.56], EntityCustomMob10000['Bandit'/6566, l='MpServer', x=25.50, y=34.00, z=8.50], EntityItemFrame['entity.ItemFrame.name'/9639, l='MpServer', x=93.50, y=74.50, z=-2.94], EntityItemFrame['entity.ItemFrame.name'/9640, l='MpServer', x=94.50, y=74.50, z=-2.94], EntitySheep['Sheep'/9641, l='MpServer', x=85.97, y=71.00, z=-8.50], EntitySheep['Sheep'/9642, l='MpServer', x=88.72, y=71.00, z=-5.91], EntitySheep['Sheep'/9643, l='MpServer', x=87.13, y=71.00, z=-0.03], EntitySheep['Sheep'/9644, l='MpServer', x=97.22, y=71.00, z=-46.50], EntitySheep['Sheep'/9645, l='MpServer', x=98.53, y=71.00, z=-46.50], EntityVillager['Villager'/9646, l='MpServer', x=88.50, y=72.00, z=14.50], EntityVillager['Villager'/9647, l='MpServer', x=88.50, y=72.00, z=15.50], EntitySheep['Sheep'/175, l='MpServer', x=22.51, y=81.00, z=-25.39], EntitySpider['Spider'/8623, l='MpServer', x=32.50, y=49.00, z=20.50], EntitySheep['Sheep'/9648, l='MpServer', x=100.53, y=69.00, z=-57.47], EntitySheep['Sheep'/176, l='MpServer', x=17.34, y=78.00, z=-40.50], EntityCreeper['Creeper'/9649, l='MpServer', x=105.00, y=20.00, z=-27.41], EntitySheep['Sheep'/177, l='MpServer', x=25.81, y=79.00, z=-23.41], EntityItem['item.tile.sapling.spruce'/9137, l='MpServer', x=65.88, y=75.13, z=-27.88], EntitySheep['Sheep'/178, l='MpServer', x=24.47, y=80.12, z=-15.56], EntitySheep['Sheep'/9651, l='MpServer', x=97.72, y=71.00, z=-14.47], EntityVillager['Villager'/9653, l='MpServer', x=86.50, y=72.00, z=30.25], EntityItem['item.tile.flowers2.minersdelight'/8885, l='MpServer', x=57.44, y=39.13, z=-7.41], EntityItem['item.tile.mushroom'/9654, l='MpServer', x=81.78, y=71.13, z=19.88], EntityVillager['Villager'/9655, l='MpServer', x=86.06, y=73.00, z=26.50], EntitySheep['Sheep'/183, l='MpServer', x=36.50, y=69.00, z=16.50], EntitySheep['Sheep'/184, l='MpServer', x=38.22, y=69.00, z=17.50], EntitySheep['Sheep'/186, l='MpServer', x=34.50, y=70.00, z=15.50], EntityItem['item.item.witchery:seedsartichoke'/7356, l='MpServer', x=-30.16, y=93.13, z=-28.19], EntitySheep['Sheep'/192, l='MpServer', x=48.97, y=75.00, z=-19.81], EntityZombie['Zombie'/8896, l='MpServer', x=-52.50, y=38.00, z=-3.50], EntitySheep['Sheep'/193, l='MpServer', x=47.63, y=76.00, z=-17.47], EntityZombie['Zombie'/8897, l='MpServer', x=-55.50, y=38.00, z=-1.50], EntitySheep['Sheep'/194, l='MpServer', x=50.88, y=74.00, z=-17.47], EntityCreeper['Creeper'/9410, l='MpServer', x=1.50, y=29.00, z=-10.50], EntityVillager['Villager'/9667, l='MpServer', x=101.66, y=71.00, z=31.41], EntityBat['Bat'/9156, l='MpServer', x=-11.72, y=37.00, z=-80.75], EntityVillager['Villager'/196, l='MpServer', x=74.50, y=72.00, z=29.16], EntityVillager['Villager'/197, l='MpServer', x=76.25, y=71.00, z=10.44], EntityItem['item.tile.sapling.spruce'/5829, l='MpServer', x=43.38, y=78.13, z=18.69], EntityVillager['Villager'/198, l='MpServer', x=81.44, y=70.00, z=4.75], EntityVillager['Villager'/199, l='MpServer', x=56.72, y=77.00, z=31.29], EntityVillager['Villager'/9672, l='MpServer', x=102.34, y=72.00, z=36.91], EntityVillager['Villager'/200, l='MpServer', x=55.88, y=77.00, z=30.31], EntityVillager['Villager'/201, l='MpServer', x=68.78, y=80.00, z=35.58], EntitySkeleton['Skeleton'/4045, l='MpServer', x=-52.56, y=85.00, z=-91.94], EntitySkeleton['Skeleton'/7631, l='MpServer', x=24.50, y=21.00, z=14.50], EntitySkeleton['Skeleton'/8660, l='MpServer', x=40.50, y=22.00, z=-43.50], EntitySpider['Spider'/8661, l='MpServer', x=42.50, y=22.00, z=-38.50], EntityItem['item.tile.flowers2.minersdelight'/5334, l='MpServer', x=11.13, y=33.13, z=-67.22], EntityCreeper['Creeper'/7127, l='MpServer', x=-33.41, y=69.00, z=-82.75], EntityZombie['Zombie'/9945, l='MpServer', x=9.50, y=20.00, z=-47.50], EntityTrail['unknown'/224, l='MpServer', x=24.69, y=76.62, z=-42.38], EntityZombie['Zombie'/9443, l='MpServer', x=59.50, y=17.00, z=-27.50], EntitySheep['Sheep'/228, l='MpServer', x=68.22, y=70.00, z=-83.50], EntitySheep['Sheep'/229, l='MpServer', x=69.81, y=71.00, z=-83.50], EntityBat['Bat'/9190, l='MpServer', x=17.73, y=54.01, z=-14.35], EntitySheep['Sheep'/230, l='MpServer', x=69.59, y=70.00, z=-79.19], EntityZombie['Zombie'/9446, l='MpServer', x=49.50, y=37.00, z=-83.50], EntitySheep['Sheep'/231, l='MpServer', x=64.06, y=70.00, z=-76.91], EntityCow['Cow'/232, l='MpServer', x=57.66, y=71.00, z=-74.31], EntityCow['Cow'/233, l='MpServer', x=58.88, y=71.00, z=-73.16], EntityZombie['Zombie'/9961, l='MpServer', x=-51.84, y=72.00, z=-71.86], EntityCow['Cow'/234, l='MpServer', x=57.47, y=71.00, z=-76.06], EntitySkeleton['Skeleton'/9962, l='MpServer', x=-41.50, y=71.00, z=-72.50], EntityCow['Cow'/235, l='MpServer', x=62.81, y=70.00, z=-79.81], EntityZombie['Zombie'/8428, l='MpServer', x=66.50, y=62.00, z=-59.50], EntityVillager['Villager'/236, l='MpServer', x=72.34, y=71.00, z=7.16], EntityZombie['Zombie'/2542, l='MpServer', x=16.78, y=63.00, z=-53.84], EntityVillager['Villager'/238, l='MpServer', x=74.50, y=72.00, z=28.28], EntitySkeleton['Skeleton'/9966, l='MpServer', x=74.50, y=59.00, z=-46.50], EntitySkeleton['Skeleton'/9967, l='MpServer', x=73.50, y=59.00, z=-45.50], EntitySkeleton['Skeleton'/9968, l='MpServer', x=75.50, y=59.00, z=-45.50], EntityItem['item.tile.sapling.spruce'/6385, l='MpServer', x=71.13, y=70.13, z=-27.88], EntityZombie['Zombie'/9970, l='MpServer', x=73.50, y=59.00, z=-47.50], EntityZombie['Zombie'/9971, l='MpServer', x=73.50, y=59.00, z=-48.50], EntityZombie['Zombie'/9972, l='MpServer', x=73.50, y=59.00, z=-44.50], EntityItem['item.item.beefRaw'/7926, l='MpServer', x=-18.75, y=83.13, z=-47.66], EntityZombie['Zombie'/6391, l='MpServer', x=43.50, y=42.00, z=-24.50], EntityArrow['arrow'/9980, l='MpServer', x=56.03, y=71.56, z=-11.03], EntityZombie['Zombie'/6655, l='MpServer', x=-26.50, y=14.00, z=22.50]]
	Retry entities: 0 total; []
	Server brand: fml,forge
	Server type: Non-integrated multiplayer server
Stacktrace:
	at net.minecraft.client.multiplayer.WorldClient.func_72914_a(WorldClient.java:373)
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2444)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:919)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)

-- System Details --
Details:
	Minecraft Version: 1.7.10
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_231, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 3008664736 bytes (2869 MB) / 4294967296 bytes (4096 MB) up to 4294967296 bytes (4096 MB)
	JVM Flags: 5 total; -Xms4096m -Xmx4096m -XX:+UseG1GC -XX:MaxGCPauseMillis=4 -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
	FML: MCP v9.05 FML v7.10.99.99 Minecraft Forge 10.13.4.1614 34 mods loaded, 34 mods active
	States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
	UCHIJA	mcp{9.05} [Minecraft Coder Pack] (minecraft.jar) 
	UCHIJA	FML{7.10.99.99} [Forge Mod Loader] (modpack.jar) 
	UCHIJA	Forge{10.13.4.1614} [Minecraft Forge] (modpack.jar) 
	UCHIJA	appliedenergistics2-core{rv3-beta-6} [Applied Energistics 2 Core] (minecraft.jar) 
	UCHIJA	appliedenergistics2{rv3-beta-6} [Applied Energistics 2] (appliedenergistics2-rv3-beta-6.jar) 
	UCHIJA	betterstorage{0.13.1.128} [BetterStorage] (BetterStorage-1.7.10-0.13.1.128.jar) 
	UCHIJA	BiomesOPlenty{2.1.0} [Biomes O' Plenty] (BiomesOPlenty-1.7.10-2.1.0.2308-universal.jar) 
	UCHIJA	BrandonsCore{1.0.0.12} [Brandon's Core] (BrandonsCore-1.0.0.12.jar) 
	UCHIJA	TwilightForest{2.3.7} [The Twilight Forest] (twilightforest-1.7.10-2.3.7.jar) 
	UCHIJA	chisel{2.9.5.11} [Chisel] (Chisel-2.9.5.11.jar) 
	UCHIJA	CarpentersBlocks{3.3.8.2} [Carpenter's Blocks] (Carpenter's+Blocks+v3.3.8.2+-+MC+1.7.10 (1).jar) 
	UCHIJA	BuildMod{v1.0} [Build Mod] (coroutil-1.1.3 for MC v1.7.10.jar) 
	UCHIJA	CoroPets{v1.0} [CoroPets] (coroutil-1.1.3 for MC v1.7.10.jar) 
	UCHIJA	CoroAI{v1.0} [CoroAI] (coroutil-1.1.3 for MC v1.7.10.jar) 
	UCHIJA	ExtendedRenderer{v1.0} [Extended Renderer] (coroutil-1.1.3 for MC v1.7.10.jar) 
	UCHIJA	ConfigMod{v1.0} [Extended Mod Config] (coroutil-1.1.3 for MC v1.7.10.jar) 
	UCHIJA	PTRModelLib{1.0.0} [PTRModelLib] (Decocraft-2.4.2_1.7.10.jar) 
	UCHIJA	props{2.4.2} [Decocraft] (Decocraft-2.4.2_1.7.10.jar) 
	UCHIJA	DraconicEvolution{1.0.2h} [Draconic Evolution] (Draconic-Evolution-1.7.10-1.0.2h.jar) 
	UCHIJA	endercore{1.7.10-0.2.0.39_beta} [EnderCore] (EnderCore-1.7.10-0.2.0.39_beta.jar) 
	UCHIJA	EnderIO{1.7.10-2.3.0.429_beta} [Ender IO] (EnderIO-1.7.10-2.3.0.429_beta.jar) 
	UCHIJA	extracells{2.3.14} [Extra Cells 2] (ExtraCells-1.7.10-2.3.14b200.jar) 
	UCHIJA	ExtraUtilities{1.2.12} [Extra Utilities] (extrautilities-1.2.12.jar) 
	UCHIJA	iChunUtil{4.2.3} [iChunUtil] (iChunUtil-4.2.3.jar) 
	UCHIJA	journeymap{5.1.4p2} [JourneyMap] (journeymap-1.7.10-5.1.4p2-unlimited.jar) 
	UCHIJA	malisiscore{1.7.10-0.14.3} [MalisisCore] (malisiscore-1.7.10-0.14.3.jar) 
	UCHIJA	malisisdoors{1.7.10-1.13.2} [Malisis' Doors] (malisisdoors-1.7.10-1.13.2.jar) 
	UCHIJA	Mantle{1.7.10-0.3.2.jenkins191} [Mantle] (Mantle-1.7.10-0.3.2b.jar) 
	UCHIJA	Morph{0.9.1} [Morph] (Morph-Beta-0.9.1.jar) 
	UCHIJA	mw{1.11.7.7} [Modern Warfare] (mw-1.11.7.7_mc1.7.10.jar) 
	UCHIJA	secretroomsmod{4.7.1} [The SecretRoomsMod] (secretroomsmod-1.7.10-4.7.1.413.jar) 
	UCHIJA	TConstruct{1.7.10-1.8.8.build991} [Tinkers' Construct] (TConstruct-1.7.10-1.8.8.build991.jar) 
	UCHIJA	tropicraft{v6.0.5} [Tropicraft] (tropicraft-6.0.5.jar) 
	UCHIJA	witchery{0.24.1} [Witchery] (witchery-1.7.10-0.24.1.jar) 
	GL info: ' Vendor: 'ATI Technologies Inc.' Version: '4.6.13572 Compatibility Profile Context 19.11.1 26.20.13031.10003' Renderer: 'Radeon RX 580 Series'
	AE2 Version: beta rv3-beta-6 for Forge 10.13.4.1448
	Mantle Environment: Environment healthy.
	TConstruct Environment: Environment healthy.
	Chisel: Errors like "[FML]: Unable to lookup ..." are NOT the cause of this crash. You can safely ignore these errors. And update forge while you're at it.
	EnderIO: Found the following problem(s) with your installation:
                  * The RF API that is being used (1.7.10R1.0.2 from <unknown>) differes from that that is reported as being loaded (1.7.10R1.0.13 from EnderIO-1.7.10-2.3.0.429_beta.jar).
                    It is a supported version, but that difference may lead to problems.
                  * An unknown AE2 API is installed (rv3 from appliedenergistics2-rv3-beta-6.jar).
                    Ender IO was build against API version rv2 and may or may not work with a newer version.
                 This may have caused the error. Try reproducing the crash WITHOUT this/these mod(s) before reporting it.
	AE2 Integration: IC2:OFF, RotaryCraft:OFF, RC:OFF, BuildCraftCore:OFF, BuildCraftTransport:OFF, BuildCraftBuilder:OFF, RF:ON, RFItem:ON, MFR:OFF, DSU:ON, FZ:OFF, FMP:OFF, RB:OFF, CLApi:OFF, Waila:OFF, InvTweaks:OFF, NEI:OFF, CraftGuide:OFF, Mekanism:OFF, ImmibisMicroblocks:OFF, BetterStorage:ON, OpenComputers:OFF, PneumaticCraft:OFF
	Launched Version: 1.7.10-Forge10.13.4.1614-1.7.10
	LWJGL: 2.9.1
	OpenGL: Radeon RX 580 Series GL version 4.6.13572 Compatibility Profile Context 19.11.1 26.20.13031.10003, ATI Technologies Inc.
	GL Caps: Using GL 1.3 multitexturing.
Using framebuffer objects because OpenGL 3.0 is supported and separate blending is supported.
Anisotropic filtering is supported and maximum anisotropy is 16.
Shaders are available because OpenGL 2.1 is supported.

	Is Modded: Definitely; Client brand changed to 'fml,forge'
	Type: Client (map_client.txt)
	Resource Packs: []
	Current Language: English (US)
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	Anisotropic Filtering: Off (1)
