
# Conexio Stratus Pro nRF9161 Device Tree for NCS v2.7.0

Before you can compile and flash the application firmware to the Stratus Pro device, 
you need to gather a few files for this board. First, we need to install the board definition 
files or the board’s devicetree in the ZephyrRTOS inside nRF Connect SDK. Zephyr utilizes devicetree to describe the 
hardware available on its supported Boards, as well as that hardware’s initial configuration. 

# Fetching Conexio Stratus Pro Board Definition Files

Since the Conexio Stratus Pro board definition files are not included in the Zephyr mainstream, developers are asked to directly download the 
board files in zip format, extract/unzip, and copy the conexio devicetree folder and place it in the NCS directory:
```
ncs/v2.7.0/zephyr/boards
```

You should now see a folder named conexio among other supported board files. Using the board 
target as `conexio_stratus_pro/nrf9161/ns` you can build Zephyr applications for the Stratus Pro board in non-secure mode.

```
└── ncs/
    └── v2.7.0/
        ├── zephyr/
        │   └── boards/
        │       ├── ...
        │       ├── ...
        │       ├── conexio
        │           └── stratus_pro
        ├── bootloader
        ├── modules
        ├── nrf
        ├── tools
        ├── toolchain
        └── ...
```

# Conexio Stratus Pro Documentation

For complete steps, see the [Conexio Documentation](https://docs.conexiotech.com/master).