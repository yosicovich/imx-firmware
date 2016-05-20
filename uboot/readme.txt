To get the source code of the uboot:
  git clone http://git.freescale.com/git/cgit.cgi/imx/uboot-imx.git

To build u-boot.imx for picoimx board:
  Assume checkout uboot code to ~/uboot-imx, brillo root dir is ~/mybrillo.
  Run below commands:
  cd ~/uboot-imx
  export ARCH=arm
  export CROSS_COMPILE=~/mybrillo/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-
  make picosom-imx6ul_defconfig
  make
