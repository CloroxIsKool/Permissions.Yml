# Permissions.Yml
Can't seem to get this file to work


This is the output log when attempted


[ERROR] [PermissionsEx]

========== UNABLE TO LOAD PERMISSIONS BACKEND =========

Your configuration must be fixed before PEX will enable

Details: Error loading permissions file!

=======================================================

ru.tehkode.permissions.exceptions.PermissionBackendException: Error loading permissions file!

at ru.tehkode.permissions.backends.file.FileBackend.reload(FileBackend.java:321) ~[PermissionsEx-1.23.4.jar:?]

at ru.tehkode.permissions.backends.file.FileBackend.<init>(FileBackend.java:120) ~[PermissionsEx-1.23.4.jar:?]

at sun.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method) ~[?:1.8.0_192]

at sun.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:62) ~[?:1.8.0_192]

at sun.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45) ~[?:1.8.0_192]

at java.lang.reflect.Constructor.newInstance(Constructor.java:423) ~[?:1.8.0_192]

at ru.tehkode.permissions.backends.PermissionBackend.getBackend(PermissionBackend.java:392) ~[PermissionsEx-1.23.4.jar:?]

at ru.tehkode.permissions.backends.PermissionBackend.getBackend(PermissionBackend.java:367) ~[PermissionsEx-1.23.4.jar:?]

at ru.tehkode.permissions.PermissionManager.createBackend(PermissionManager.java:624) ~[PermissionsEx-1.23.4.jar:?]

at ru.tehkode.permissions.PermissionManager.setBackend(PermissionManager.java:606) ~[PermissionsEx-1.23.4.jar:?]

at ru.tehkode.permissions.PermissionManager.initBackend(PermissionManager.java:693) ~[PermissionsEx-1.23.4.jar:?]

at ru.tehkode.permissions.PermissionManager.<init>(PermissionManager.java:67) ~[PermissionsEx-1.23.4.jar:?]

at ru.tehkode.permissions.bukkit.PermissionsEx.onEnable(PermissionsEx.java:175) [PermissionsEx-1.23.4.jar:?]

at org.bukkit.plugin.java.JavaPlugin.setEnabled(JavaPlugin.java:265) [spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.bukkit.plugin.java.JavaPluginLoader.enablePlugin(JavaPluginLoader.java:347) [spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.bukkit.plugin.SimplePluginManager.enablePlugin(SimplePluginManager.java:410) [spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.bukkit.craftbukkit.v1_13_R2.CraftServer.enablePlugin(CraftServer.java:436) [spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.bukkit.craftbukkit.v1_13_R2.CraftServer.enablePlugins(CraftServer.java:350) [spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at net.minecraft.server.v1_13_R2.MinecraftServer.l(MinecraftServer.java:580) [spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at net.minecraft.server.v1_13_R2.MinecraftServer.a(MinecraftServer.java:542) [spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at net.minecraft.server.v1_13_R2.MinecraftServer.a(MinecraftServer.java:420) [spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at net.minecraft.server.v1_13_R2.DedicatedServer.init(DedicatedServer.java:294) [spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at net.minecraft.server.v1_13_R2.MinecraftServer.run(MinecraftServer.java:698) [spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at java.lang.Thread.run(Thread.java:813) [?:1.8.0_192]

Caused by: org.bukkit.configuration.InvalidConfigurationException: mapping values are not allowed here

in 'string', line 3, column 12:

default: true

^

at org.bukkit.configuration.file.YamlConfiguration.loadFromString(YamlConfiguration.java:57) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at ru.tehkode.permissions.backends.file.FileConfig.loadFromString(FileConfig.java:68) ~[?:?]

at org.bukkit.configuration.file.FileConfiguration.load(FileConfiguration.java:163) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.bukkit.configuration.file.FileConfiguration.load(FileConfiguration.java:131) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at ru.tehkode.permissions.backends.file.FileConfig.load(FileConfig.java:38) ~[?:?]

at ru.tehkode.permissions.backends.file.FileBackend.reload(FileBackend.java:309) ~[?:?]

... 23 more

Caused by: org.yaml.snakeyaml.scanner.ScannerException: mapping values are not allowed here

in 'string', line 3, column 12:

default: true

^

at org.yaml.snakeyaml.scanner.ScannerImpl.fetchValue(ScannerImpl.java:870) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.scanner.ScannerImpl.fetchMoreTokens(ScannerImpl.java:358) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.scanner.ScannerImpl.checkToken(ScannerImpl.java:227) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.parser.ParserImpl$ParseBlockMappingKey.produce(ParserImpl.java:558) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.parser.ParserImpl.peekEvent(ParserImpl.java:158) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.parser.ParserImpl.checkEvent(ParserImpl.java:148) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.composer.Composer.composeMappingNode(Composer.java:214) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.composer.Composer.composeNode(Composer.java:144) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.composer.Composer.getNode(Composer.java:85) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.composer.Composer.getSingleNode(Composer.java:108) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.constructor.BaseConstructor.getSingleData(BaseConstructor.java:139) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.Yaml.loadFromReader(Yaml.java:524) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.yaml.snakeyaml.Yaml.load(Yaml.java:437) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.bukkit.configuration.file.YamlConfiguration.loadFromString(YamlConfiguration.java:55) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at ru.tehkode.permissions.backends.file.FileConfig.loadFromString(FileConfig.java:68) ~[?:?]

at org.bukkit.configuration.file.FileConfiguration.load(FileConfiguration.java:163) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at org.bukkit.configuration.file.FileConfiguration.load(FileConfiguration.java:131) ~[spigot-1.13.2.jar:git-Spigot-e6eb36f-d3ed151]

at ru.tehkode.permissions.backends.file.FileConfig.load(FileConfig.java:38) ~[?:?]

at ru.tehkode.permissions.backends.file.FileBackend.reload(FileBackend.java:309) ~[?:?]

... 23 more

[INFO] [PermissionsEx] Disabling PermissionsEx v1.23.4
