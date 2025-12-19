# State-Of-Play
Last update: 2025-12-09 &mdash; 1.21.11 supported

This page contains occasional updates to the status of SlimeDog plugins,
with particular reference to compatibility with newer versions of Minecraft.

SlimeDog plugins were transitioned to End Of Life (EOL) on 2024-07-09,
meaning that development and support ceased, and the source code and wiki pages were locked.
At that point, SlimeDog plugins were compatible with Minecraft 1.21,
and they remained 100% compatible through Minecraft 1.21.3.
The following sections show the status of each plugin for newer versions of Minecraft servers and proxies.

💬 If you are an experienced developer, interested in adopting any SlimeDog plugin, please leave a note in the [issues](https://github.com/SlimeDog/State-Of-Play/issues) section.

-----

## AggressiveAnimals 1.9.0
✅ Compatible with PaperMC: through 1.21.11 <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ⚠️ Ghast variants introduced in 1.21.6 are not supported: [ghastling](https://minecraft.wiki/w/Ghastling), [happy ghast](https://minecraft.wiki/w/Happy_Ghast) <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ⚠️ Passive mobs introduced in 1.21.11 are not supported:
[camel husk](https://minecraft.wiki/w/Camel_Husk),
[nautilus](https://minecraft.wiki/w/Nautilus),
[zombie horse](https://minecraft.wiki/w/Zombie_Horse) <br>
⛔ Incompatible with SpigotMC 1.21.4 and later &mdash; MC version is not supported <br>

## BiomeRemap 3.2.4
✅ Compatible with PaperMC and SpigotMC: through 1.21.11 <br>

## EntityCount 1.2.0
✅ Compatible with PaperMC and SpigotMC: through 1.21.11 <br>

## MobColors 1.2.0
✅ Compatible with PaperMC and SpigotMC: through 1.21.11 <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ⚠️ Cold, temperate, and warm variants introduced in 1.21.5 are not supported: [chicken](https://minecraft.wiki/w/Chicken#Variants), [cow](https://minecraft.wiki/w/Cow#Variants), [pig](https://minecraft.wiki/w/Pig#Variants) <br> 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ⚠️ Ghast variants introduced in 1.21.6 are not supported: [ghastling](https://minecraft.wiki/w/Ghastling), [happy ghast](https://minecraft.wiki/w/Happy_Ghast) <br>

## NetworkInterceptor 3.4.3
✅ Compatible with PaperMC and SpigotMC: through 1.21.11 <br>
✅ Compatible with BungeeCord 1.21-* <br>
✅ Compatible with Velocity 3.4.0-* <br>
⚠️ Configuration and start-up modification required for Java 24 <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &mdash; Security Manager is permanently disabled in Java 24 and following; see [release note](https://openjdk.org/jeps/486) <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &mdash; Consequently, NetworkInterceptor method `security-manager` is no longer supported <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &mdash; Delete (or comment out) `security-manager` at line 32 of [config.yml](https://github.com/SlimeDog/NetworkInterceptor/blob/master/src/main/resources/config.yml) <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &mdash; Start server or proxy without the optional Java parameter `-Djava.security.manager=allow` <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &mdash; Some outgoing requests will no longer be recognized, as described at line 27 of [config.yml](https://github.com/SlimeDog/NetworkInterceptor/blob/master/src/main/resources/config.yml) <br>

## pHD 1.9.0
✅ Compatible with PaperMC and SpigotMC: through 1.21.11 <br>
<!-- &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ⚠️ 1.21.9 compatibility waiting for updates to hologram providers <br> -->

## PluginVersions 1.3.5
✅ Compatible with PaperMC and SpigotMC: through 1.21.11 <br>
✅ Compatible with BungeeCord 1.21-* <br>
✅ Compatible with Velocity 3.4.0-* <br>
