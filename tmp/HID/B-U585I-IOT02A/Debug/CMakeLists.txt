# CMSIS Build CMakeLists generated on 2024-05-06T15:57:52

cmake_minimum_required(VERSION 3.22)

# Target options

set(TARGET HID)
set(CPU Cortex-M33)
set(PRJ_DIR "c:/Test/USBD/HID")
set(OUT_DIR "C:/Test/USBD/out/HID/B-U585I-IOT02A/Debug")
set(INT_DIR "C:/Test/USBD/tmp/HID/B-U585I-IOT02A/Debug")
set(FPU SP_FPU)
set(DSP DSP)
set(TZ TZ)
set(SECURE TZ-disabled)
set(BYTE_ORDER Little-endian)
set(OPTIMIZE none)
set(DEBUG on)
set(AS_FLAGS_GLOBAL "-masm=auto")
set(CC_FLAGS_GLOBAL "-std=gnu11 -Wno-macro-redefined -Wno-pragma-pack -Wno-parentheses-equality -Wno-license-management")
set(CXX_FLAGS_GLOBAL "-Wno-macro-redefined -Wno-pragma-pack -Wno-parentheses-equality -Wno-license-management")
set(LD_FLAGS_GLOBAL "--entry=Reset_Handler --map --info summarysizes --summary_stderr --diag_suppress=L6314W")
set(LD_SCRIPT "c:/Test/USBD/Board/B-U585I-IOT02A/RTE/Device/STM32U585AIIx/ac6_linker_script.sct.src")
set(LD_REGIONS "c:/Test/USBD/Board/B-U585I-IOT02A/RTE/Device/STM32U585AIIx/regions_B-U585I-IOT02A.h")
set(LD_SCRIPT_PP "C:/Test/USBD/tmp/HID/B-U585I-IOT02A/Debug/ac6_linker_script.sct")

set(DEFINES
  STM32U585xx
  _RTE_
  USE_FULL_LL_DRIVER
  USE_HAL_DRIVER
)

set(INC_PATHS
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Inc"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Inc/Legacy"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/CMSIS/Device/ST/STM32U5xx/Include"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Inc"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/MX_Device/Board"
  "c:/Test/USBD/HID/RTE/CMSIS"
  "c:/Test/USBD/HID/RTE/USB"
  "c:/Test/USBD/HID/RTE/_Debug_B-U585I-IOT02A"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-Compiler/2.0.0/include"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Include"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS/6.0.0/CMSIS/Core/Include"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS/6.0.0/CMSIS/Driver/Include"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS/6.0.0/CMSIS/Driver/VIO/Include"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS/6.0.0/CMSIS/RTOS2/Include"
  "C:/w/MDK-Middleware/USB/Include"
  "C:/w/MDK-Middleware/USB/Source/Include"
)

set(ASM_SRC_FILES
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/GCC/irq_armv8mml.S"
)

set(AS_ARM_SRC_FILES
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/MDK-ARM/startup_stm32u585xx.s"
)

set(CC_SRC_FILES
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-Compiler/2.0.0/source/armcc/retarget_io.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_delay.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_evflags.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_evr.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_kernel.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_lib.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_memory.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_mempool.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_msgqueue.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_mutex.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_semaphore.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_system.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_thread.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS-RTX/5.8.0/Source/rtx_timer.c"
  "C:/Users/reikei01/AppData/Local/Arm/Packs/ARM/CMSIS/6.0.0/CMSIS/RTOS2/Source/os_systick.c"
  "C:/w/MDK-Middleware/USB/Include/usbd_config.c"
  "C:/w/MDK-Middleware/USB/Include/usbd_debug.c"
  "C:/w/MDK-Middleware/USB/Source/usb_lib_ver.c"
  "C:/w/MDK-Middleware/USB/Source/usbd_lib_core.c"
  "C:/w/MDK-Middleware/USB/Source/usbd_lib_core_device.c"
  "C:/w/MDK-Middleware/USB/Source/usbd_lib_core_hid.c"
  "C:/w/MDK-Middleware/USB/Source/usbd_lib_drv.c"
  "C:/w/MDK-Middleware/USB/Source/usbd_lib_hid.c"
  "C:/w/pack-examples/B-U585I-IOT02A_BSP/CMSIS/Driver/vio_B-U585I-IOT02A.c"
  "C:/w/pack-examples/STM32U5xx_DFP/CMSIS/Driver/IrDA_STM32U5xx.c"
  "C:/w/pack-examples/STM32U5xx_DFP/CMSIS/Driver/OTG_STM32U5xx.c"
  "C:/w/pack-examples/STM32U5xx_DFP/CMSIS/Driver/SmartCard_STM32U5xx.c"
  "C:/w/pack-examples/STM32U5xx_DFP/CMSIS/Driver/UART_STM32U5xx.c"
  "C:/w/pack-examples/STM32U5xx_DFP/CMSIS/Driver/USART_STM32U5xx.c"
  "C:/w/pack-examples/STM32U5xx_DFP/CMSIS/Driver/USBD_OTG_STM32U5xx.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_cortex.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_dma.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_dma_ex.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_exti.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_flash.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_flash_ex.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_gpio.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_gtzc.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_i2c.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_i2c_ex.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_icache.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_mdf.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_ospi.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_pcd.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_pcd_ex.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_pwr.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_pwr_ex.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_rcc.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_rcc_ex.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_spi.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_spi_ex.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_tim.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_tim_ex.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_uart.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_hal_uart_ex.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_ll_dlyb.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_ll_dma.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_ll_exti.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_ll_gpio.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_ll_lpgpio.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_ll_ucpd.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_ll_usb.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Drivers/STM32U5xx_HAL_Driver/Src/stm32u5xx_ll_utils.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Src/main.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Src/stm32u5xx_hal_msp.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Src/stm32u5xx_hal_timebase_tim.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Src/stm32u5xx_it.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/CubeMX/STM32CubeMX/Src/system_stm32u5xx.c"
  "c:/Test/USBD/Board/B-U585I-IOT02A/retarget_stdio.c"
  "c:/Test/USBD/HID/HID.c"
  "c:/Test/USBD/HID/RTE/CMSIS/RTX_Config.c"
  "c:/Test/USBD/HID/USBD_User_HID_0.c"
)

# Toolchain config map

set(REGISTERED_TOOLCHAIN_ROOT "c:/Users/reikei01/.vcpkg/artifacts/2139c4c6/compilers.arm.armclang/6.22.0/bin")
set(REGISTERED_TOOLCHAIN_VERSION "6.22.0")
set(TOOLCHAIN_VERSION_MIN "6.22.0")
include ("C:/Keil_v5/ARM/cmsis-toolbox/etc/AC6.6.18.0.cmake")
include ("C:/Keil_v5/ARM/cmsis-toolbox/etc/CMSIS-Build-Utils.cmake")

# Setup project

project(${TARGET} LANGUAGES ASM AS_ARM C)

cbuild_get_running_toolchain(TOOLCHAIN_ROOT TOOLCHAIN_VERSION C)

# Global Flags

set(CMAKE_ASM_FLAGS "${ASM_CPU} ${ASM_BYTE_ORDER} ${ASM_DEFINES} ${ASM_OPTIONS_FLAGS} ${ASM_FLAGS} ${AS_FLAGS_GLOBAL}")
set(CMAKE_AS_ARM_FLAGS "${AS_ARM_CPU} ${AS_ARM_BYTE_ORDER} ${AS_ARM_DEFINES} ${AS_ARM_OPTIONS_FLAGS} ${AS_ARM_FLAGS} ${AS_FLAGS_GLOBAL}")
cbuild_get_system_includes(CC_SYS_INC_PATHS_LIST CC_SYS_INC_PATHS)
set(CMAKE_C_FLAGS "${CC_CPU} ${CC_BYTE_ORDER} ${CC_DEFINES} ${CC_SECURE} ${CC_OPTIONS_FLAGS} ${CC_FLAGS} ${CC_FLAGS_GLOBAL} ${CC_SYS_INC_PATHS}")
set(CMAKE_C_LINK_FLAGS "${LD_CPU} ${_LS}\"${LD_SCRIPT_PP}\" ${LD_SECURE} ${LD_FLAGS_GLOBAL} ${LD_OPTIONS_FLAGS} ${LD_FLAGS}")

# Local Flags

foreach(SRC ${ASM_SRC_FILES})
  set_source_files_properties(${SRC} PROPERTIES LANGUAGE ASM)
endforeach()

foreach(SRC ${AS_ARM_SRC_FILES})
  set_source_files_properties(${SRC} PROPERTIES LANGUAGE AS_ARM)
endforeach()

# Compilation Database

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
add_custom_target(database COMMAND ${CMAKE_COMMAND} -E copy_if_different "${INT_DIR}/compile_commands.json" "${OUT_DIR}")

# Setup Target

add_executable(${TARGET} ${ASM_SRC_FILES} ${AS_ARM_SRC_FILES} ${CC_SRC_FILES})
set_target_properties(${TARGET} PROPERTIES PREFIX "" SUFFIX ".axf" OUTPUT_NAME "HID")
set_target_properties(${TARGET} PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${OUT_DIR} LINK_DEPENDS ${LD_SCRIPT})
target_include_directories(${TARGET} PUBLIC ${INC_PATHS})

# Linker script pre-processing

add_custom_command(TARGET ${TARGET} PRE_LINK COMMAND ${CPP} ARGS ${CPP_ARGS_LD_SCRIPT} BYPRODUCTS ${LD_SCRIPT_PP})
