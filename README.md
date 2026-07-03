# Spawn Invulnerability (Fabric, Minecraft 26.2)

Restores the ~3 second invulnerability players used to get when joining a
world or respawning after death. This was vanilla behavior for years and was
removed in Minecraft 1.21.4.

- Requires: Fabric Loader 0.19.3+, Fabric API for 26.2, Java 25, Minecraft 26.2
- Configurable via game rule: `/gamerule spawninvuln:spawn_invulnerability_ticks <ticks>`
  (20 ticks = 1 second, default is 60 = 3 seconds, 0 disables it)

## How to get the .jar file (no local install needed)

1. Create a free account at https://github.com if you don't have one.
2. Create a new repository and upload every file/folder from this project
   (or push it with git if you're comfortable with that).
3. Go to the "Actions" tab of your repository. A build will start
   automatically (or click "Run workflow" if it doesn't).
4. Wait for the green checkmark, open the finished run, and download the
   "Artifacts" file at the bottom - that's a zip containing your `.jar`.
5. Put that `.jar` file, plus a matching Fabric API `.jar` for 26.2, into your
   `.minecraft/mods` folder.

## Building locally instead (if you do have Java installed)

```
./gradlew build
```

The finished jar will be in `build/libs/`.
