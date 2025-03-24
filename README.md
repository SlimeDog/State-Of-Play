# State-Of-Play
Last update: 2025-03-23

This page contains occasional updates to the status of SlimeDog plugins,
with particular reference to compatibility with newer versions of Minecraft.

SlimeDog plugins were transitioned to End Of Life (EOL) on 2024-07-09,
meaning that development and support have ceased.
At that point, they were compatible with Minecraft 1.21,
and they remained 100% compatible through Minecraft 1.21.3.
The following sections show the status of each plugin on the date shown above.

-----

## AggressiveAnimals
- Compatible with PaperMC 1.21.4
- ⚠️ Incompatible with SpigotMC 1.21.4 or later &mdash; new MC version is not recognized

## BiomeRemap
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4

## EntityCount
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4

## MobColors
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4
- ⚠️ Mob variants introduced in 1.21.5 are not recognized: [chicken](https://minecraft.wiki/w/Chicken#Variants), [cow](https://minecraft.wiki/w/Cow#Variants), [pig](https://minecraft.wiki/w/Pig#Variants)

## NetworkInterceptor
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4
- ⚠️ Requires configuration modification on Java 24
  - `Security Manager` was [permanently removed](https://openjdk.org/jeps/486) in Java 24
  - NetworkInterceptor method `security-manager` is no longer available for use
    - It should be deleted (or commented out) at line 32 of [config.yml](https://github.com/SlimeDog/NetworkInterceptor/blob/master/src/main/resources/config.yml)
  - Some outgoing requests will no longer be recognized, as described at line 27 of [config.yml](https://github.com/SlimeDog/NetworkInterceptor/blob/master/src/main/resources/config.yml)

## pHD
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4

## PluginVersions
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4

