# V4L2 testing application

## Version 0.1.0

## Build

```
$ mkdir build
$ cd build
$ cmake -DCMAKE_BUILD_TYPE:STRING=Release ..
$ cmake --build .
```

## Build for aarch64 targets (cross compile)
```
$ sudo apt update
$ sudo apt install binutils-aarch64-linux-gnu g++-aarch64-linux-gnu
$ mkdir build
$ cd build
$ cmake -DCMAKE_BUILD_TYPE:STRING=Release -DCMAKE_C_COMPILER:FILEPATH=/home/volpi/gcc/bin/aarch64-none-linux-gnu-gcc -DCMAKE_CXX_COMPILER:FILEPATH=/home/volpi/gcc/bin/aarch64-none-linux-gnu-g++ ..
$ cmake --build . ; scp v4l2-test root@10.41.4.133:/home/root/
```