# Realtek 8812BU Driver for Raspbian

Driver for 802.11ac USB adapter with RTL8812BU chipset, only STA/Monitor mode is supported, no AP mode.

A few known wireless cards that use this driver include:
* [Fastoe AC1300 USB Wi-Fi Adapter](https://www.amazon.com/Adapter-1300Mbps-Raspberry-Supports-Raspbain/dp/B081TGWCVB/ref=as_li_ss_tl?dchild=1&m=A9879GOT1YWJ2&marketplaceID=ATVPDKIKX0DER&qid=1602768172&s=merchant-items&sr=1-6&linkCode=ll1&tag=fastoe-20&linkId=fe3481ad40b60930c6b909d00c179510&language=en_US)
* Cudy WU1200 AC1200 High Gain USB Wi-Fi Adapter

Currently tested with Linux RaspberryPi 5.4.51-v7l+/4.19.118-v7+/4.19.97-v7+ on:
- Raspberry Pi 4 B
- Raspberry Pi 3 B+

### Manual installation

To build, you have to retrieve source and run `make`.
If via Git, do following:

```bash
sudo apt-get install git bc raspberrypi-kernel-headers
git clone https://github.com/fastoe/RTL8812BU_for_Raspbian
cd RTL8812BU_for_Raspbian
make
sudo make install
sudo reboot
```

Enjoy!
