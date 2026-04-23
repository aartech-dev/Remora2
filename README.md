# The AART&trade;,  Remora&trade; 2 Slot Car eCom

This git repo contains the files you need to make a Remora 2 slot car electronic commutator (eCom) at [JLCPCB](https://jlcpcb.com). 

The files were exported from KiCad and are in the ["production" directory](https://github.com/aartech-dev/Remora2/tree/main/production) in this repo. They comprise:

  - the [Gerber Files](https://github.com/aartech-dev/Remora2/blob/main/production/Remora2.0.zip)
  - the [Bill of Materials file](https://github.com/aartech-dev/Remora2/blob/main/production/bom.csv) [JLCPCB example](https://jlcpcb.com/help/article/bill-of-materials-for-pcb-assembly) 
  - the [Pick and Place file](https://github.com/aartech-dev/Remora2/blob/main/production/positions.csv) [JLCPCB example](https://jlcpcb.com/help/article/pick-place-file-for-pcb-assembly)

By downloading these files you implicitly need to agree with the associated [modified Open Source license agreement](https://github.com/aartech-dev/Remora2/blob/main/AART_Remora_eCom_License_v2.0.pdf).

The ESCape32 binaries are in the [bin directory](https://github.com/aartech-dev/Remora2/tree/main/bin). The build targets are:

    add_target(BOOT3_PA2_FE STM32F0 AT32F4 IO_PA2 IO_RXTX FAST_EXIT)    

    add_target(AART2 AT32F421 TIMING=15 FREQ_MIN=48 FREQ_MAX=96 DUTY_RATE=20 DUTY_SPUP=20 DEAD_TIME=24 COMP_MAP=123 ARM= 0 VOLUME=0 INPUT_MODE=1 ANALOG_CHAN=6 ANALOG_MIN=0 ANALOG_MAX=1440 DUTY_MIN=100 FULL_DUTY)    
