# notes
Assorted notes

## Initial Configuration

- sudo raspi-config
- # expand filesystem (nic neudelalo)
- # generate locale for cs-CZ
- # change GPU memory to 4M
- # switch kernel to use device tree
- # enable SPI
- # enable I2C

# DEVELOPMENT dependencies
```bash
sudo apt-get install \
    i2c-tools
```

## ...

# Exporting udev database
```bash
udevadm info --export-db > udev
```

# XWindows forwarding in sudo

```bash
sudo visudo
# add Defaults        env_keep += "DISPLAY HOME XAUTHORITY"
vim ~/.profile
# add export XAUTHORITY="$HOME/.Xauthority"
```

# Enabling i2c 

```bash
# add
i2c-bcm2708
i2c-dev
# to
sudo vim /etc/modules
```

create /etc/udev/rules.d/80-orchidarium.rules



