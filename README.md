## Fix Edimax dongle

- Download this driver (8188eu.ko).
- Replace the driver on the EV3 in the `/lib/modules/4.14.117-ev3dev-2.3.5-ev3/drivers/net/wireless/` folder. (Make a backup, just in case!)
- Reboot the EV3.
- Insert the WiFi-dongle into the device once it has started.
- Check that the WiFi-option is still empty.
- Execute (on the EV3) `sudo modprobe 8188eu`.
- To automatically enable it on startup, add 8188eu to `/etc/modules`.
- The WiFi should now be available on the EV3-brick. Use either the UI or the commandline to connect to a network
