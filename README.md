> This is a forked verson to work on ThinkBook 14+ 2022, or other devices with 174f:1811 Syntek Integrated Camera.

# chicony-ir-toggle
This project aims to control the IR emitters of windows hello enabled IR cameras under Linux. See https://github.com/boltgolt/howdy/issues/269 for a discussion and background about the methods used.

## Installation

Using cmake
```
mkdir -p build
cd build
cmake ..
make
sudo make install
```

Using gcc
```
gcc main.c -o chicony-ir-toggle
```

## Usage

```
chicony-ir-toggle [-d DEVICE] <on|off>
```
Default for DEVICE is `/dev/video2`. If this differs on your system, supply the `-d` command line parameter pointing to your video device.


