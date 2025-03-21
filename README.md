# State-Of-Play
Last update: 2025-03-20

This page contains occasional updates to the status of SlimeDog plugins,
with particular reference to compatibility with newer versions of Minecraft.

SlimeDog plugins were transitioned to End Of Life (EOL) on 2024-07-09.
at which point they were compatible with Minecraft 1.21.
They remained compatible through Minecraft 1.21.3.

## AggressiveAnimals
- Compatible with 1.21.3 PaperMC and SpigotMC
- ⚠️ Compatible with 1.21.4 PaperMC only

## BiomeRemap
- Compatible with 1.21.4 PaperMC and SpigotMC

## EntityCount
- Compatible with 1.21.4 PaperMC and SpigotMC

## MobColors
- Compatible with 1.21.4 PaperMC and SpigotMC <br>
- ⚠️ Unaware of mob variants introduced in 1.21.5 for chicken, cow, pig

## NetworkInterceptor
- Compatible with 1.21.4 PaperMC and SpigotMC
- ⚠️ Requires configuration modification on Java 24
  - Security Manager was permanently removed in Java 24
  - NetworkInterceptor method security-manager is no longer recognized, and should be deleted: line 32 of the canonical config.yml
  - Some outgoing requests will not be recognized by NetworkInterceptor method proxy-selector, as described in the canonical config.yml

## pHD
- Compatible with 1.21.4 PaperMC and SpigotMC

## PluginVersions
- Compatible with 1.21.4 PaperMC and SpigotMC

