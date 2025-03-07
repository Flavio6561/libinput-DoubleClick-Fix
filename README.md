## libinput-DoubleClick-Fix,
A script that removes the default double click ghosting in libinput  
```
sudo mkdir -p /etc/libinput
sudo sh -c 'echo "[libinput-DoubleClick-Fix]
MatchUdevType=mouse
ModelBouncingKeys=1" > /etc/libinput/local-overrides.quirks'
```
