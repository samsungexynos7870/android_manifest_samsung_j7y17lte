# Aosp

### How to build ###

```bash
# Create dirs
$ mkdir aosp ; cd aosp

# Init repo
$ repo init --depth=1 -u https://github.com/crdroidandroid/android.git -b 10.0

# Clone my local repo
$ git clone https://github.com/batuhantrkgl/android_manifest_samsung_j7y17lte.git -b aosp .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ . build/envsetup.sh && lunch lineage_j7y17lte-userdebug && mka clean && mka api-stubs-docs && mka hiddenapi-lists-docs && mka system-api-stubs-docs && mka test-api-stubs-docs && mka bacon -j`nproc`
```

## Credits
2019 @Astrako
2022 @Batuhantrkgl

## Contact
Telegram support group: https://t.me/joinchat/D1Jk_VbieGBXOWZt2y8O7A
Telegram Support Group: https://t.me/Exynos7870Updates
