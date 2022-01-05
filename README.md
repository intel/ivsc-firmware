# ivsc-firmware

This repository supports Intel Vision Sensing Controller(IVSC) on Intel Alder Lake
platforms. There are two repositories that provide the complete setup:

- https://github.com/intel/ivsc-driver - kernel driver for the ivsc chipset
- https://github.com/intel/ivsc-firmware - firmware binaries for the ivsc chipset

## Content of this repository:
- ivsc firmware binaries

## Deployment
ivsc firmware binaries should be copied to /lib/firmware/vsc

And on debugging platform the binaries(e.g. ov01a10 sensor) should be copied as below:
```
/lib/firmware/vsc/soc_a1/ivsc_fw_a1.bin
/lib/firmware/vsc/soc_a1/ivsc_pkg_ovti01a0_0_a1.bin
/lib/firmware/vsc/soc_a1/ivsc_skucfg_ovti01a0_0_1_a1.bin
```

And on production platform the binaries(e.g. ov01a10 sensor) should be copied as below:
```
/lib/firmware/vsc/soc_a1_prod/ivsc_fw_a1_prod.bin
/lib/firmware/vsc/soc_a1_prod/ivsc_pkg_ovti01a0_0_a1_prod.bin
/lib/firmware/vsc/soc_a1_prod/ivsc_skucfg_ovti01a0_0_1_a1_prod.bin
```
