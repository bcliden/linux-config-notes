### Basic nvidia tools and options

legacy: `optirun`

future: `primusrun`

verbose mode: `optirun|primusrun -v`

see if NVIDIA CARD is running:
`cat /proc/acpi/bbswitch`

can also run
`glxgears -info`

to configure the nvidia driver:
`optirun -b none nvidia-settings -c :8`

### to open the VGA display and keep the service in the terminal:

`primusrun intel-virtual-output -b`

`optirun intel-virtual-output -b`

use `-f` flag to prevent daemonization

`fn + F7` to open display modal
