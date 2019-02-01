# linux-cortexm-tools  
- JLink_Linux_V642_x86_64.deb  
  官网：[https://www.segger.com/downloads/jlink/#J-LinkSoftwareAndDocumentationPack](#https://www.segger.com/downloads/jlink/#J-LinkSoftwareAndDocumentationPack)  
  这是Ubuntu系统下的J-Link安装包。  
  双击直接运行安装。  
  【01】执行 JLinkExe 命令行运行J-Link。  
  【02】执行 connect 命令链接j-Link调试器。  
  【03】设置参数。  
  【04】loadbin FileFullPath Address  

- OpenOCD  
  一个开源项目，在Ubuntu上可以直接安装。  
  【01】sudo apt-get install openocd  
  【02】openocd -f interface/jlink.cfg -f target/stm32f4x.cfg  
  【03】打开另一个窗口  
  【04】telnet localhost 4444  
  【05】halt  
  【06】flash write_image erase example/stm32f407_led/stm32f407_led.hex  

- arm-none-eabi-  
  ARM官网[https://developer.arm.com/open-source/gnu-toolchain/gnu-rm/downloads](#https://developer.arm.com/open-source/gnu-toolchain/gnu-rm/downloads)  
  这是一个交叉编译工具链。
