# Lync-GPS
Notes from the Lync GPS peer locator devices. USB captures and more

## Useful things:
Blog post about the tool I used: https://lynqme.com/blogs/articles/a-software-update-gps-assist-are-now-available-with-lynq-updater

I've run a USB capture while using the GPS Assist tool. I clicked the GPS Assist button 10 seconds after the device said it added successfully (~14s) and repeated this process 4 times. The USBCaptureSummary file is just a text dump of the view I have in wireshark.

USBCommands.md is my documentation of the commands and responses that I've seen thus far.

## Help needed
Open the pcap and identify more things from it. Packets 333-347(odd packets only) appear to be the Lynq firmware updater tool sending the "GPS Assist" command that tells the device to start looking in this roughly 70mi area when it begins aquiring a signal.

Packets 349-359 (odd only again) are the reponse. Is that just GPS coords? Why are there several sent? Is that a square area?
