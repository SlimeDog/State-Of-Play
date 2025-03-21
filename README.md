# State-Of-Play
Last update: 2025-03-20

This page contains occasional updates to the status of SlimeDog plugins,
with particular reference to compatibility with newer versions of Minecraft.

SlimeDog plugins were transitioned to End Of Life (EOL) on 2024-07-09.
at which point they were compatible with Minecraft 1.21.
They remained compatible through Minecraft 1.21.3.

## AggressiveAnimals
- Compatible with PaperMC 1.21.4
- ⚠️ Incompatible with SpigotMC 1.21.4 or later

## BiomeRemap
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4

## EntityCount
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4

## MobColors
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4
- ⚠️ Unaware of mob variants introduced in 1.21.5 for chicken, cow, pig

## NetworkInterceptor
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4
- ⚠️ Requires configuration modification on Java 24
  - Security Manager was permanently removed in Java 24
  - NetworkInterceptor method security-manager is no longer recognized, and should be deleted: line 32 of the canonical config.yml
  - Some outgoing requests will not be recognized by NetworkInterceptor method proxy-selector, as described in the canonical config.yml

## pHD
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4

## PluginVersions
- Compatible with PaperMC 1.21.4 and SpigotMC 1.21.4

