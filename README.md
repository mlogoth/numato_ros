
Add the following line to the ```/etc/udev/rules.d/99-custom.rules``

```sh
SUBSYSTEM=="tty",ACTION=="add", ATTRS{idVendor}=="2a19", ATTRS{idProduct}=="0802", MODE="0777", SYMLINK+="ttyNUMATO"
```

