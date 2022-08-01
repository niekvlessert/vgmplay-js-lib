# vgmplay-js-lib

Project to get to emscripten transpiled libvgm based library for playing VGM files, using an audioworklet.

Currently it's based on vgmplay and using the old scriptprocessor. Other versions will be in other branches. Building should work with actions, result should be on github.io

The index.html includes a very bary demo, it just plays.

Run it on a https webserver (thisisunsafe for Chrome errors on a local ssl webserver, please google...).

- Visit the page: https://ip/vgmplay-js-lib/
- Press load
- Press play

A music file is included in the data file which is generated in the compilation process.

Building:

```
cd /var/www/html/
git clone --recursive https://github.com/niekvlessert/vgmplay-js-lib.git
cd vgmplay-js-lib
mkdir build
cd build
emcmake cmake ..
make
cp *.data ..
```
