 
in `/etc/X11/xorg.conf.d/20-thinkpad.conf`

Section "InputClass"
	Identifier	"Trackpoint Wheel Emulation"
	MatchProduct	"TPPS/2 IBM TrackPoint|DualPoint Stick|Synaptics Inc. Composite TouchPad / TrackPoint|ThinkPad USB Keyboard with TrackPoint|USB Trackpoint pointing device|Composite TouchPad / TrackPoint"
	MatchDevicePath	"/dev/input/event*"
	Option		"EmulateWheel"		"true"
	Option		"EmulateWheelButton"	"2"
	Option		"Emulate3Buttons"	"false"
	Option		"XAxisMapping"		"6 7"
	Option		"YAxisMapping"		"4 5"
	Option 		"AccelSpeed"		"-0.40"
EndSection

added udev rules in `/etc/udev/rules.d/10-trackpoint.rules`

ACTION="add",
SUBSYSTEM="input",
ATTR{name}=="TPPS/2 IBM TrackPoint",
ATTR{device/sensitivity}="132",
ATTR{device/speed}="158",
ATTR{device/inertia}="6",
ATTR{device/rate}="200",
ATTR(device/press_to_select}="0"

later changed to:

ACTION="add",
SUBSYSTEM="input",
ATTR{name}=="TPPS/2 IBM TrackPoint",
ATTR{device/sensitivity}="138",
ATTR{device/speed}="97",
ATTR{device/inertia}="6",
ATTR{device/rate}="200",
ATTR(device/press_to_select}="0"
