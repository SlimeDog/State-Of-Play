# State-Of-Play
Occasion updates to status of SlimeDog plugins, which are EOL/archived

Last update: 2025-03-20

AggressiveAnimals
- Compatible with 1.21.4 on PaperMC only; throws an error on SpigotMC

BiomeRemap
- Compatible with 1.21.4

EntityCount
- Compatible with 1.21.4

MobColors
- Compatible with 1.21.4
- Unaware of variations introduced in 1.21.5: chicken, cow, pig

NetworkInterceptor
- Compatible with 1.21.4
- Requires configuration modification on Java 24
  - Security Manager was premanently disabled in Java 24
  - NetworkInterceptor method security-manager is no longer recognized, and should be deleted: line 32 of canonical config.yml
  - Some outgoing requests will not be recognized by NetworkInterceptor method proxy-selector

pHD
- Compatible with 1.21.4

PluginVersions
- Compatible with 1.21.4

