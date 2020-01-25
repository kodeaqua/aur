### Android Unpack Repack
A tool for un/repack Android's filesystem from Termux
Written by Adam Najmi Zidan

### Version
1.0 - Initial release

### Requirements
1. At least you need more than 3GB free space at Internal Storage. Btw, it depends on your project. My kenzo has 2560M system partition. So, i always keep my Internal Storage has 4-5GB free space.
2. Internet connection. You'll need up to 20mB to install/upgrade termux package(s)
3. Knowledge about Android Porting

### Special Thanks
1. [Andrei Conache (xpirt)](https://github.com/xpirt)
2. [Jake Valletta (jakev)](https://github.com/jakev)
3. [Rendi Stiawan (rendiix)](https://github.com/rendiix)

### How to install
if you're new in Termux, you must install git before installing AUR
``` console
$ pkg install git
```
Then clone AUR repo
``` console
$ git clone https://github.com/user-ilang/aur.git
```
Change into AUR dir
``` console
$ cd aur
```
Change AUR modes, so you can execute it
``` console
$ chmod +x aur
```
Run AUR, then wait till installation done
``` console
$ ./aur
```

### How to use
Run as termux-root
``` console
$ tsu
```
Create dir for your project
``` console
# mkdir <project-name>
```
Change into your project dir
``` console
# cd <project-name>
```
Run aur script :D
``` console
# aur
```
Then push your stuff into your project dir via any rootexplorer app.
1. system.img or vendor.img (raw image only, not sparse image/simg type)
2. system.new.dat(.br), system.patch.dat, system.transfer.list
3. vendor.new.dat(.br), vendor.patch.dat, vendor.transfer.list
4. file_contexts.bin or file_contexts (Important, but if you don't have, no problem)
AUR will automatically detecting system or vendor and image or dat.
And don't worry if you've (.br) compressed dat, AUR will decompress it :)
