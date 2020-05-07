# sm64pc
OpenGL adaptation of [n64decomp/sm64](https://github.com/n64decomp/sm64). 

## Building

### On Linux

#### 1. Copy baserom(s) for asset extraction

For each version (jp/us/eu) that you want to build a ROM for, put an existing ROM at
`./baserom.<version>.z64` for asset extraction.

#### 2. Install build dependencies

The build system has the following package requirements:
  * python3 >= 3.6
  * libsdl2-dev
  * [audiofile](https://audiofile.68k.org/)
  * libglew-dev
  * git


__Debian / Ubuntu - targeting 32 bits__
```
sudo apt install build-essential git python3 libaudiofile-dev libglew-dev:i386 libsdl2-dev:i386
```
__Debian / Ubuntu - targeting 64 bits__
```
sudo apt install build-essential git python3 libaudiofile-dev libglew-dev libsdl2-dev
```

## Current issues

 * Support for the EU version is still experimental.
 * There seems to be savedata-related problems on some 64-bits builds.
