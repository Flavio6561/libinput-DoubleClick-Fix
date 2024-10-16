## libinput-DoubleClick-Fix,
A script that removes double click delay/ghosting in distros using libinput  
### How to use:
- Run the [downloaded file](https://github.com/Flavio6561/libinput-DoubleClick-Fix/releases/download/v.1.0.0/libinput-DoubleClick-Fix.sh) or
- Copy and run the code here:
```
sudo mkdir -p /etc/libinput  
sudo sh -c 'echo "[libinput-DoubleClick-Fix]  
MatchUdevType=mouse  
ModelBouncingKeys=1" > /etc/libinput/local-overrides.quirks'
```
### What does the code do?
- `sudo mkdir -p /etc/libinput`: creates the directory, `-p` to avoid errors in case the directory already exists  
- `sudo sh -c '...'`: runs all the code in the apostrophes (`''`) with root permissions  
- `echo "[libinput-DoubleClick-Fix]` `MatchUdevType=mouse` `ModelBouncingKeys=1" > /etc/libinput/local-overrides.quirks`: prints in the terminal and uses it as a string to redirect the output to `/etc/libinput/local-overrides.quirks`  

**Note: old overrides will be overwritten**
