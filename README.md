
![layout image][layout_image]

Following Instruction is from [github.com/kiibohd/wiki][firmware_instruction]

# Mac OSX

* Open a terminal
* May require root permissions
* Using brew (recommended) or macports, install "dfu-util" (`brew install dfu-util` or `port install dfu-util` and `port install libusb`)
* Enter DFU Flash Mode (e.g. press flash button), the debug led will turn on.
* Flash using `dfu-util -D <.dfu.bin>`
* Debug led will turn off
* Keyboard is ready!


# Linux

Unfortunately/fortunately, there are a large number of Linux distributions.
Below is the currently list of tested Linux distributions.
If you know how to successfully load firmware on another distribution, please add it here :D 
In general it should be as simple as installing `dfu-util`.

* Plug in keyboard
* Open a terminal
* May require root permissions
* Install dfu-util package (see distro section below)
* Enter DFU Flash Mode (e.g. press flash button), the debug led will turn on.
* Flash using `dfu-util -D <.dfu.bin>`
* Debug led will turn off
* Keyboard is ready!


## Ubuntu / Debian

```bash
sudo apt-get install dfu-util
```


## Arch Linux

```bash
sudo pacman -Sy dfu-util
```


## Fedora

```bash
sudo yum install dfu-util
```


## OpenSuse

```bash
sudo zypper install dfu-util
```


# Other

Loading DFU firmware from other OSs has not been tested.
In most cases however as long as there is dfu-util available for your platform it should be possible.
If you are successful, please add it here :D

[firmware_instruction]: https://github.com/kiibohd/controller/wiki/Loading-DFU-Firmware
[layout_image]: layout.png
