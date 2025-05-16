![Banner](https://github.com/user-attachments/assets/2ee33ef5-f45f-4ea6-8780-9086905c493a)

# Project Flare | Reborn from ashes of Project Blaze
An Android Operating System Based On AOSP.

### Requirements
- Around 500GB disk space.
- Around 32GB RAM running Linux.

### Sync our source ###
```bash
repo init -u https://github.com/Project-Flare-Staging/manifest -b 15 --git-lfs
```
```bash
repo sync -c --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```

### Build our source ###

- Set up the build environment
```bash
source build/envsetup.sh
```

- Lunch a target
```bash
lunch flare_$devicecodename-bp1a-userdebug
```

- To start compiling
```bash
make bacon -j$(nproc --all)
```
