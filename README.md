mymdf2iso
==========================================

A port of the [mdf2iso](http://freshmeat.sourceforge.net/projects/mdf2iso/) tool by Salvatore Santagati to Windows (CodeBlocks/Mingw64).

There is already a windows build out there, but the original and existing ports have an issue where they write the progress bar to the terminal for every single byte leading to taking forever to convert an image (several minutes).

This port only updates the progress bar when the percent changes. That makes conversion take a few seconds (on an SSD), it's basically as fast as your drive can write the iso file out.

Tested on a PSX game in a PC emulator (converted mds/mdf to cue/bin then started it).

Usage: mdf to cue/bin

```
mymdf2iso.exe --cue file.mdf
```

