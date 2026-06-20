# MSD-BootLoader
Black Pill Mass Storage Device BootLoaders 32F411CE


LoadeR ViTa - 16K Virtual FAT Table

Start Adress for User code: 0x08004000

Pressing KEY and connect to USB for BootLoader start

The new Interrupt Vector Table is already set up before the jump


Loader PRM - 32K

Start Adress for User Code: 0x08008000

BotLoader will start if there is communication with USB

The new Interrupt Vector Table is already set up before the jump

Rename Disk Volume to "SAVE" for saving FAT Table

Rename Disk Volume to "SAVE to F0VL" for saving FAT Table with parameters

Loader PRM Parameters:

F - save PLL frequency after jump (CPU: 96MHz, USB,APB1,APB2: 48Mz)

V - VBUS sensetive. Start BootLoader if user pin is '1'

0..9 - set user key / user pin line PA0..PA9

L - Lock last Sector for writing

For Example: "SAVE to L0FA"

Lock last 128K sector for writing

Starts Bootloader by '0' at PA0

Save RCC frequency for user programm

'A' - it doesn't matter
