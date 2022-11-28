# snap-cameractrls

Unofficial [snapcraft](https://snapcraft.io) build files for the [cameractrls](https://github.com/soyersoyer/cameractrls) Linux camera command line and GUI.

To permit access to your webcam, the `camera` interface needs to be first connected:

```bash
snap connect cameractrls:camera :camera
```

The `cameractrls.cameractrlsgtk` command is the GTK GUI while `cameractrls` is
the command line client:

```
$ cameractrls -d
option -d requires argument
usage: /snap/cameractrls/x1/usr/bin/cameractrls.py [--help] [-d DEVICE] [--list] [-c CONTROLS]

optional arguments:
  -h, --help         show this help message and exit
  -d DEVICE          use DEVICE, default /dev/video0
  -l, --list         list the controls and values
  -L, --list-devices list capture devices
  -c CONTROLS        set CONTROLS (eg.: hdr=on,fov=wide)

example:
  /snap/cameractrls/x1/usr/bin/cameractrls.py -c brightness=128,kiyo_pro_hdr=on,kiyo_pro_fov=wide
```

[![cameractrls]()](https://snapcraft.io/cameractrl)
