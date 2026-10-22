# Porting notes

This is a source-level backport of Satin Free Wakes to Minecraft 1.20.1 Fabric.

## Upstream revisions

- Satin-free source fork: [Commander07/wakes](https://github.com/Commander07/wakes), commit `178434ab8fe36e655cb54b3490962825e4b19fdf`.
- Original Wakes 1.20.1 reference branch: [Goby56/wakes, 1.20.1](https://github.com/Goby56/wakes/tree/1.20.1), commit `b9dc5fb4e9ee32a4a16a1fb5b94e4bf56ddba4d3`.

## Compatibility changes

- Retargeted Minecraft, Yarn, Fabric API, Mod Menu, and Iris compile-time compatibility to their 1.20.1 variants.
- Adapted particle types and particle geometry callbacks to the 1.20.1 API.
- Restored the 1.20.1 buffer-builder and shader-supplier APIs while retaining the satin-free emissive wake rendering path.
- Updated model helpers, color packing, world-height lookup, and the boat paddle access widener for 1.20.1.
- Kept YetAnotherConfigLib optional at runtime; Mod Menu shows its fallback prompt when YACL is absent.

The original GPL license is included unchanged. Upstream authors remain credited in `fabric.mod.json`; `JustHari01` is credited for this backport.
