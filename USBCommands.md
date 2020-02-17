# USB Commands
These are commands observed from USB captures.
## Basic info
Pcap5 good filtering: `usb.device_address eq 7 and usb.bus_id eq 1 and usb.capdata != ""`
## Get GPS version
Command from USB host:
usb.capdata: 474554564552
Translated:
GETVER

Response:
```
24424547494e4f464745545645520d0a
312e31322e3030312e340d0a
24444f4e450d0a
```

Translated:
```
$BEGINOFGETVER\r\n
1.12.001.4\r\n
$DONE\r\n
```

## ???
Command from USB host:
`4c594e513031324152484d`

Translated:
`LYNQ012ARHM`

Response:
```
24544f47474c45434f4d4d414e44530d0a
24444f4e455f4750530d0a
```
Translated:
```
$TOGGLECOMMANDS\r\n
$DONE_GPS\r\n
```

Response2:
```
24544f47474c45434f4d4d414e44530d0a
24444f4e455f49444c450d0a
```
Translated2:
```
$TOGGLECOMMANDS\r\n
$DONE_IDLE\r\n
```
