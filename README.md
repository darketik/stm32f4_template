stm32f4_template
================

Eclipse template project for:
- stm43f40_41xx microcontroller 
- configured for gcc arm none eabi toolchain with C++ support
- containing:
  - CMSIS library with DSP lib, cortex-m4 lib, startup.S, system_stm32f4.h/c and stm32f40_41xxx.h
  - STM32F40_41xx Discovery dev board library
  - Some STM32F4 USB drivers (OTG, Device HID)
  - linker, openocd and gdb scripts 
  - STM32F4 standard peripherals drivers
- Defined symbols:
  USE_STDPERIPH_DRIVER
  USE_STM32F4_DISCOVERY
  STM32F40_41xxx
  __VFP_FP__     not sure to be necessary, to be checked
  __FPU_PRESENT=1
  ARM_MATH_CM4
  HSE_VALUE=8000000
  (USEOTG_MODE
  USE_HOST_MODE
  USE_USB_OTG_FS
  
-  !! Warning !! : Don't forget to change binary name into gdb script 'stm32f407vg_flash_and_debug.script'
before calling it.

