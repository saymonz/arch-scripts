# systemd-boot-mkconfig
Bash script for autogeneration of systemd-boot entry files

Use at your own risk.

There is various settings on script beginning. Run as root (or sudo). This scripts assumes that your /boot partition is your EFI partition. If not, you will have to copy the init ramdisks and kernels by yourself.

It detects installed kernels and generates systemd-boot loader entries. You have to edit the script with your own kernel parameters. The script generates two entries for each kernel: default and fallback.

It should not interfere with existing entries if you specify a prefix in the script.

I'm very new to Bash scripting so maybe your computer will explode, I take no responsability.
