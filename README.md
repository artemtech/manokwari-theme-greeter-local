# LightDM-Webkit Greeter Theme for BlankOn
## DEPENDENCIES
You have to install ```lightdm-webkit-greeter``` firstly from repository on your Linux,

[ArchLinux Based - install from AUR]
```bash
$ yaourt -S lightdm-webkit2-greeter
```
[Debian Based]
```bash
$ sudo apt install lightdm-webkit-greeter
```

## HOW-TO MANUAL INSTALL ON VARIOUS DISTRO:
1.
```bash
$ git clone https://github.com/artemtech/manokwari-theme-greeter
$ cd manokwari-theme-greeter
manokwari-theme-greeter$ sudo cp greeter /usr/share/lightdm-webkit/themes/manokwari-theme-greeter
```
2. edit file ```/etc/lightdm/lightdm-webkit-greeter.conf``` and fill up ```webkit-theme``` entry with ```manokwari-theme-greeter```
3. edit file ```/etc/lightdm/lightdm.conf``` find: `#greeter-session=` change it to `greeter-session=lightdm-webkit-greeter`
or
if there is no entries in lightdm.conf, you can directly add by yourself:
```bash
[Seat:*]
greeter-session=lightdm-webkit-greeter```
