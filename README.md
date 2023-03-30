# Godot Evdev

Godot Evdev is a native GDExtension for Godot 4.x that exposes libevdev functionality
to GDSCript. It allows you to directly access and process input events from
`/dev/input/event*` devices and create virtual devices using uinput.

## Requirements

### Build Requirements

The following are required to build Open Gamepad UI:

- Godot 4.x
- GCC 7+ or Clang 6+.
- Python 3.5+.
- SCons 3.0+ build system
- pkg-config (used to detect the dependencies below).
- X11, Xcursor, Xinerama, Xi and XRandR development libraries.
- MesaGL development libraries.
- ALSA development libraries.
- PulseAudio development libraries.
- Evdev development libraries
- make (optional)
- unzip (optional)
- wget (optional)

If you are using ArchLinux, you can run the following:

```bash
pacman -S --needed scons pkgconf gcc libxcursor libxinerama libxi libxrandr mesa glu libglvnd alsa-lib pulseaudio libevdev make unzip wget git
```

## Building

You can build the project using the following:

```bash
make build
```

## Usage

Copy the `addons` folder after you have built the project into your Godot
project directory.
