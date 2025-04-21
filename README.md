# OrangeFox Action Builder
Compile your first custom recovery from OrangeFox Recovery using Github Action.

# How to Use
1. Fork this repository.

2. Get your kernel and push it using github desktop or by git, to device/brand/codename/kernel/brand/chip-number/ (change brand to your phone brand, codename to your phone's codename, DO NOT change kernel, change brand to the brand of your phone again, and change chip-build to your chip's model number like sm7325 which is the Snapdragon 778G 5G Mobile Platform. Example directory: device/nothing/Spacewar/kernel/nothing/sm7325 )

3. Go to `Action` tab > `All workflows` > `OrangeFox - Build` > `Run workflow`, then fill all the required information:
 * MANIFEST_BRANCH (`12.1` and `11.0`)
 * DEVICE_TREE (Your device tree repository link.)
 * DEVICE_TREE_BRANCH (Your device tree repository branch.)
 * DEVICE_PATH (`device/vendor/codename`)
 * DEVICE_NAME (Your device codename)
 * BUILD_TARGET (`boot`, `recovery`, `vendorboot`)

 # Note
* This action will now only support manifest 12.1 and 11.0, since all orangefox manifest below 11.0 are considered obsolete.
* Make sure your tree uses right variable (updated vars) from OrangeFox; [fox_11.0](https://gitlab.com/OrangeFox/vendor/recovery/-/blob/fox_11.0/orangefox_build_vars.txt) and [fox_12.1](https://gitlab.com/OrangeFox/vendor/recovery/-/blob/fox_12.1/orangefox_build_vars.txt), to avoid build erros.

Credits to @NothingOSS for the kernel, @carlodandan for the builder, and @Maitreya25 and [@DeathGamerB] for the builder.
