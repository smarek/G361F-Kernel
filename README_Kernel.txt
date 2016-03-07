################################################################################

1. How to Build
	- get Toolchain
		From android git server , codesourcery and etc ..
		 - aarch64-linux-android-4.8
		
	- edit Makefile
		edit target architecture.
	    - ARCH = arm64
		edit "CROSS_COMPILE" to right toolchain path(You downloaded).
		  EX)  CROSS_COMPILE= $(android platform directory you download)/android/prebuilts/gcc/linux-x86/aarch64/aarch64-linux-android-4.8/bin/aarch64-linux-android-
      Ex)  CROSS_COMPILE=/usr/local/toolchain/aarch64-linux-android-4.8/bin/aarch64-linux-android-          // check the location of toolchain
  	
		$ make pxa1908_coreprimevelte_eur_defconfig
		$ make

2. Output files
	- Kernel : arch/arm64/boot/Image

3. How to Clean	
		$ make clean
################################################################################
