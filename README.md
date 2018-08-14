# android_device_motorola_peregrine-twrp
To build android 8.1 branch

Initialise a repo with the following command

"repo init -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni -b twrp-8.1"

Add the included peregrine_manifest.xml to the .repo/local_manifests folder (create it if it doesn't exist)

Then "repo sync"

Then, "source build/envsetup.sh" --> "lunch omni_peregrine-eng" --> "mka recoveryimage -j4"

You can change the 4 in -j4 to suit the number of threads in your system
