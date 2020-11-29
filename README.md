# Game Development Final Project

## Design Doc:
https://docs.google.com/document/d/1Ewje6-3yslvrHLfv-ThOgXNSGMK_r2XTRdlrzRGZzR4/edit?usp=sharing

## Meeting Minutes:
https://docs.google.com/document/d/1QekhMSTy6Pz9g_gSK4FYyHnuOj7aJYdjck2Hv8T_fJM/edit?usp=sharing

## Team Members:
Aayush Gupta
<br>Azeezah Muhammad
<br>Bradley Aboua
<br>Nikesh Subedi

## How to pull code and push changes:
This project is large and so some parts are broken off into [submodules](https://gist.github.com/gitaarik/8735255).  The project is designed to run even if you don't have space to download all submodules.

### Current Submodules:
 - FinalProject/Content/Characters (https://github.com/Azeezah/BananaBoxCharacters)

Use the following commands to pull and push code.

### To pull everything:
```
git config alias.update '!git pull && git submodule update --init'
git update
```
Now you can use `git update` instead of `git pull`.  This will download code for all of the submodules along with the main repository.

### To pull a smaller version of the project (with no submodules):
```
git pull
```

### To pull a smaller version of the project (with some submodules):
```
git pull

cd FinalProject/Content/Characters    # Or the folder of whichever submodule you'd like to pull.
git submodule init
git config alias.update '!git pull && git submodule update'
```
Now you can use `git update` instead of `git pull`.  This will download code for all **initialized** submodules along with the main repository.

### To push code:
Use `git push` the way you normally would.
 - Running `git push` inside the submodule's folder will push code to the corresponding repository.
 - Otherwise, it'll push to this repo as usual.
