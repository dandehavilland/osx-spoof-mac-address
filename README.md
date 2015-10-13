# osx-spoof-mac-address

I recently left my bittorrent client open and active (down/uploading totally
legit data ofcourse...) whilst connected to a free café network. Thanks to this, my MAC
address was blackisted. Ooops.

After a little research, I could put together this script which assigns a new,
random MAC address to your **en0** & **en1** interfaces.

Tested and working on:
- OSX Yosemite 10.10.5, MacBook Pro 13-inch Mid-2010.

I welcome your reports of working/not working, please file an issue.

## Usage

- Turn off Wifi
- `./spoof-mac-address`
- Enter sudo password when prompted
- Turn on Wifi
- Surf.

This only works for one session: once you've restarted your machine the old MAC
address will return.

Note: Occasionally the new MAC address will not be accepted by the system. I
think this is down to some odd/even characters being in the wrong place. If at
first you don't succeed, try again.

## Disclaimer

I take no responsibility for any damage to your system. Use at your own risk!
