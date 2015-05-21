# Map Development #
Map development is done using a bit modified java version of tiled editor http://www.mapeditor.org/ sources can be found
[here](http://valkyrie.firegnom.com/downloads/Tiled-Valkyrie.tar.gz) .

Right now there are not many modifications done to this editor and map making in it is a bit crude , but i hope it is a great
base for map editor and later on after some modifications map making will be much  easier.


## How to Start ##
All map files and tools are located in graphics repository located
[here](http://code.google.com/p/valkyrie-android/source/browse?repo=valkyrie-graphics) to start map development you need to clone it.


```
	hg clone https://valkyrie-graphics.valkyrie-android.googlecode.com/hg/ valkyrie-android-valkyrie-graphics
```

Start editor :
To run this editor java needs to be installed and java needs to be in path

On linux just run **mapEditor.sh** and on windows **mapEditor.bat**


## Rules ##

  1. all maps need to have tileset named `_moveMatrix`
  1. tileset `_moveMatrix` needs to have image `moveMatrix.png`
  1. all maps need to have layer named `_moveMatrix` and only tileset used on this layer can be from `_moveMatrix` tileset
  1. all context actions can be in written in Object group layer Named `_ContextActions`
  1. there can be only one layer named `_ContextActions`


## Moves ##
Move matrix shows where player can go and where he can't right now red  mens player can't enter.

## Scripting ##
Scripting is done using [BeenShell](http://www.beanshell.org/)

sample script :
```
if (player.distance(p) > 5)
	gui.toast("you are to far");
else
	gui.info("I never liked to cut trees they are so peacefull harmless i hate to kill them ");
```

more comming soon...

## Tips ##
Best way to start is to open already existing map the one which is right now a main is named : introv9-ver\_4.tmx.gz