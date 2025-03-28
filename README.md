# State-Of-Play
Last update: 2025-03-28

This page contains occasional updates to the status of SlimeDog plugins,
with particular reference to compatibility with newer versions of Minecraft.

SlimeDog plugins were transitioned to End Of Life (EOL) on 2024-07-09,
meaning that development and support have ceased.
At that point, they were compatible with Minecraft 1.21,
and they remained 100% compatible through Minecraft 1.21.3.
The following sections show the status of each plugin for newer versions of Minecraft servers and proxies.

-----

## AggressiveAnimals 1.9.0
✅ Compatible with PaperMC 1.21.4 <br>
⛔ Incompatible with SpigotMC 1.21.4 and later &mdash; MC version is not supported <br>

## BiomeRemap 3.2.4
✅ Compatible with SpigotMC 1.21.5 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>

## EntityCount 1.2.0
✅ Compatible with SpigotMC 1.21.5 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>

## MobColors 1.2.0
✅ Compatible with SpigotMC 1.21.5 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>
⚠️ Mob variants introduced in 1.21.5 are not supported: [chicken](https://minecraft.wiki/w/Chicken#Variants), [cow](https://minecraft.wiki/w/Cow#Variants), [pig](https://minecraft.wiki/w/Pig#Variants) <br>

## NetworkInterceptor 3.4.3
✅ Compatible with SpigotMC 1.21.5 <br>
✅Compatible with BungeeCord 1.21-1929 <br>
✅ Compatible with Velocity 3.4.0-483 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>
⚠️ Configuration modification required for Java 24 <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &mdash; Security Manager is permanently disabled in Java 24 and following; see [release note](https://openjdk.org/jeps/486) <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &mdash; Consequently, NetworkInterceptor method `security-manager` is no longer supported <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &mdash; Delete (or comment out) `security-manager` at line 32 of [config.yml](https://github.com/SlimeDog/NetworkInterceptor/blob/master/src/main/resources/config.yml) <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &mdash; Start server or proxy without the optional Java parameter `-Djava.security.manager=allow` <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &mdash; Some outgoing requests will no longer be recognized, as described at line 27 of [config.yml](https://github.com/SlimeDog/NetworkInterceptor/blob/master/src/main/resources/config.yml) <br>

## pHD 1.9.0
✅ Compatible with SpigotMC 1.21.5, verified with DecentHolograms 2.8.16 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>

## PluginVersions 1.3.5
✅ Compatible with SpigotMC 1.21.5 <br>
✅ Compatible with BungeeCord 1.21-1929 <br>
✅ Compatible with Velocity 3.4.0-483 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>
