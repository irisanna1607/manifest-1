# ANDROID OPEN SOURCE EXTENDED PROJECT 
 ============================================================================
A custom Android firmware exclusively for supporting devices whose
OEM has been abandoned with latest software and security implementation.

# CREDITS
---------
nikhil sir
neenu miss

# How to Build?
-------------

To initialize your local repository using the AOSEP trees, use a 
command like this:

```bash
  repo init -u git://github.com/ExtendedOS/manifest.git -b pie
...
  
Then to sync up:
----------------

```bash
  repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
Finally to build:
-----------------

```bash
  . build/envsetup.sh
  lunch aosp_device_codename-userdebug
  mka aosep -j$(nproc --all)
  where j$ denotes the number of available cores
  ...
