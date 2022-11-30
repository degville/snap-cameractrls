# snap-cameractrls

Unofficial [snapcraft](https://snapcraft.io) build files for the [cameractrls](https://github.com/soyersoyer/cameractrls) Linux camera command line and GUI.

To permit access to your webcam, the `camera` interface needs to be first connected:

```bash
snap connect cameractrls:camera
```

To permit access to out-of-spec camera options, such as HDR mode on the Kiyo Pro, connect the raw-usb interface:

```bash
snap connect cameractrls:raw-usb
```

From the desktop, launching `cameractrls` will launch the GTK GUI version.

The `cameractrls.cameractrlsgtk` command is the GTK GUI while `cameractrls` is
the command line client:

```
$ cameractrls
usage: /snap/cameractrls/x8/usr/bin/cameractrls.py [--help] [-d DEVICE] [--list] [-c CONTROLS]

optional arguments:
  -h, --help         show this help message and exit
  -d DEVICE          use DEVICE, default /dev/video0
  -l, --list         list the controls and values
  -L, --list-devices list capture devices
  -c CONTROLS        set CONTROLS (eg.: hdr=on,fov=wide)

example:
  /snap/cameractrls/x8/usr/bin/cameractrls.py -c brightness=128,kiyo_pro_hdr=on,kiyo_pro_fov=wide
```

[![cameractrls](https://snapcraft.io/cameractrls/badge.svg)](https://snapcraft.io/cameractrls)
