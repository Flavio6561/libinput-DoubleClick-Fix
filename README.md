## libinput-DoubleClick-Fix,
A script that removes double click delay/ghosting in Linux distros using libinput  
### How to use:
- Copy and run the script:
```
sudo mkdir -p /etc/libinput
sudo sh -c 'echo "[libinput-DoubleClick-Fix]
MatchUdevType=mouse
ModelBouncingKeys=1" > /etc/libinput/local-overrides.quirks'
```
**Note: old overrides will be overwritten**
