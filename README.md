# State-Of-Play
Last update: 2025-03-27

This page contains occasional updates to the status of SlimeDog plugins,
with particular reference to compatibility with newer versions of Minecraft and proxies.

SlimeDog plugins were transitioned to End Of Life (EOL) on 2024-07-09,
meaning that development and support have ceased.
At that point, they were compatible with Minecraft 1.21,
and they remained 100% compatible through Minecraft 1.21.3.
The following sections show the status of each plugin for newer of Minecraft and proxies.

-----

## AggressiveAnimals
✅ Compatible with PaperMC 1.21.4 <br>
⛔ Incompatible with SpigotMC 1.21.4 or later &mdash; MC version is not supported <br>

## BiomeRemap
✅ Compatible with SpigotMC 1.21.5 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>

## EntityCount
✅ Compatible with SpigotMC 1.21.5 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>

## MobColors
✅ Compatible with SpigotMC 1.21.5 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>
⚠️ Mob variants introduced in 1.21.5 are not supported: [chicken](https://minecraft.wiki/w/Chicken#Variants), [cow](https://minecraft.wiki/w/Cow#Variants), [pig](https://minecraft.wiki/w/Pig#Variants) <br>

## NetworkInterceptor
✅ Compatible with SpigotMC 1.21.5 <br>
✅Compatible with BungeeCord 1.21-1929 <br>
✅ Compatible with Velocity 3.4.0-483 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>
⚠️ Configuration modification requires for Java 24 <br>
  - `Security Manager` was [permanently removed](https://openjdk.org/jeps/486) in Java 24
  - NetworkInterceptor method `security-manager` is no longer supported
    - `security-manager` should be deleted (or commented out) at line 32 of [config.yml](https://github.com/SlimeDog/NetworkInterceptor/blob/master/src/main/resources/config.yml)
  - Some outgoing requests will no longer be recognized, as described at line 27 of [config.yml](https://github.com/SlimeDog/NetworkInterceptor/blob/master/src/main/resources/config.yml)

## pHD
✅ Compatible with SpigotMC 1.21.5, verified with DecentHolograms 2.8.16 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>

## PluginVersions
✅ Compatible with SpigotMC 1.21.5 <br>
✅ Compatible with BungeeCord 1.21-1929 <br>
✅ Compatible with Velocity 3.4.0-483 <br>
✅ Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4 <br>
