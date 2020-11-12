Popcorn Linux for Distributed Thread Execution
----------------------------------------------

## Cross compilation for ARM64

Change -j to use twice the number of cores.

```bash
$ cat config_blue_popcorn > .config 
$ make -j16 ARCH=arm64 CROSS_COMPILE=aarch64-linux-gnu- distclean 
$ make -j16 ARCH=arm64 CROSS_COMPILE=aarch64-linux-gnu- menuconfig # Make sure Popcorn is enabled
$ make -j16 ARCH=arm64 CROSS_COMPILE=aarch64-linux-gnu-  
```

* Visit http://popcornlinux.org and https://github.com/ssrg-vt/popcorn-kernel/wiki for more information including copyright.
