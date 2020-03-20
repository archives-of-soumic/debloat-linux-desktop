# debloat-linux-desktop
When you install a fresh linux distro (`Debian` in my case), it comes with pre-installed apps. 
Though some of the apps are useful, some of them are never used. Removing them one-by-one is a 
slow process. So in order to automate this process, I thouhgt to make this script. 

Basically I scrolled through the software store, marked the apps, tracked down the package names 
from the terminal (`$ apt search <possible-package-name>`), created a list and finally put them
in a script. So a single command removes these bloats very easily.

I have tested this on my laptop running `Debian 10 testing` with `Cinnamon` desktop environment. However, this should work on any Debian/Ubuntu based distro.

# warning 
1. If you use any of these apps, please edit the script by simply removing the package names 
that you use, save it and then run it. Please refer to the `apps that are removed` section for 
a list of apps.
2. While running the script, please read the line saying 
```
The following packages will be REMOVED:
  lightning thunderbird ... ...
```
If you see something suspecious, such as `cinnamon-desktop-environment`, or equivalent Gnome, 
KDE, XFCE packages, donot run it as your desktop environment may crash.
# usage
Download the repository. There is a file named `debloat.sh`, simply run it.
```
$ git clone https://github.com/fahimfarhan/debloat-linux-desktop.git
$ cd debloat-linux-desktop
$ chmod +x debloat.sh
$ sudo ./debloat.sh
```

# apps that are removed
The following packages will be removed:
* thunderbird
* cheese 
* gnome-klotski 
* gnome-mahjongg 
* gnome-mines 
* gnome-robots 
* gnome-sudoku 
* gnome-tetravex 
* quadrapassel 
* tali 
* lightsoff 
* swell-foop 
* hexchat 
* gnome-nibbles

