Before we get to the point of all that packet sniffing goodness... a word of warning
from the people who actually did all the work.

# WARNING

The scripts in this repo may damage your hardware and may void your hardware’s warranty! 
You use these scripts and the tools from https://github.com/seemoo-lab/nexmon at your own risk and responsibility! 
If you don't like these terms, don't use nexmon!
If you don't like these terms, don't run any of the scripts in this repo.

# SECOND WARNING

Seriously, use of these scripts in this RaspPiNexmonScripts Repo could brick your raspberry pi and render it useless.
The scrits in this Repo automate the work done at https://github.com/seemoo-lab/nexmon who also warn that your hardware
could suffer irreperable and permenent damage.

Only carry on if you take full responsibility.

I have only automated the RasPi steps described in detail at https://github.com/seemoo-lab/nexmon


# RaspPiNexmonScripts for Kernel 4.14 only.

## Raspberry Pi, set built in chip to monitor mode. (Pi-Zero W, Pi-3B and Pi-3B+)

The good people at the following link, the nexmon project have instructions to 
compile a modified driver to unlock the onboard wifi chip on the raspberry pi.

https://github.com/seemoo-lab/nexmon

### Script:  WiFiCardModDriver.sh

I've automated that process with a script that you can run on the following RasPi models

-Pi Zero W (Hardware revision 9000c1)

-Pi Model 3B (Hardware revision a02082, a22082  & a32082)

-Pi Model 3B+ (Hardware revision a020d3)


The script will detect and build the modified driver for the above models.
The script will backup the origional hardware driver from location, 
/lib/modules/4.14.79-v7+/kernel/drivers/net/wireless/broadcom/brcm80211/brcmfmac/brcmfmac.ko
to
/lib/modules/4.14.79-v7+/kernel/drivers/net/wireless/broadcom/brcm80211/brcmfmac/brcmfmac.ko.bkp

RUN AS ROOT

For board revision history information, you might like to check the following link,

https://elinux.org/RPi_HardwareHistory#Board_Revision_History



