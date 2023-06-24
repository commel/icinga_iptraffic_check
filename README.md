# Icinga Check for openSUSE's zypper

## Requirements
This check only requires Python 3.6 (openSUSE Leap 15.4 based) and nothing
more. Place it somewhere accessible for Icinga.

## Arguments

	./check_iptraffic -deth0

* -d name of the monitored device

## Installation
Place the check_iptraffic somewhere where Icinga can access it (e.g. /usr/local/bin). Then append the
content of ```services.conf``` and ```commands.conf``` to your Icinga files.

## Config
Put this in your ```host.conf```:

```
        vars.iptraffic_devices["eth0"] = {
                iptraffic_device = "eth0"
        }

```


