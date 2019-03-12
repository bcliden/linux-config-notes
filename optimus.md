 
legacy: `optirun`

future: `primusrun`

verbose mode: `optirun|primusrun -v` 

see if NVIDIA CARD is running:
`cat /proc/acpi/bbswitch`

can also run 
`glxgears -info`

to configure the nvidia driver:
`optirun -b none nvidia-settings -c :8`
