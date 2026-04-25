# Excuse the spaghetti
This repo is currently an absolute mess and I'm trying to move everything online so collaboration is easier. Updated CAD and EasyEDA drawings (currently being ported from KiCad) will be available soon.

# What is this project?
There have been a lot of fantastic and open-source DAP designs popping up recently, but nothing that has quite scratched my itch for a more modern and capable iPod-style DAP. While [tangara](https://www.crowdsupply.com/cool-tech-zone/tangara) and the [Echo R1](https://github.com/amachronic/echoplayer) both look like fantastic devices, they don't quite meet my wants from a modern DAP. 
To me, the platonic ideal for a DAP is the iPod Video. Unfortunately, despite having spent tons of time and money dealing with iPods, they aren't always reliable, and fixing them can be really expensive. 
This project aims to recreate the iPod Video experience in a modern chassis with improved and repairable hardware, native RockBox support and comprehensive documentation for anyone looking to repair or contribute.

# What are those requirements?

- RockBox: The fantastic people of [RockBox](https://www.rockbox.org/) made the arguably best firmware for most music players. Starting from scratch with a documented system and common MCU should be boons to any developers

- OLED: While the focus of a DAP is music, a nice screen is always a plus. OLED offers much higher brightness compared to LCD displays and reduced power draw if using a dark UI. This used to be unfeasible, but new 2.7" OLED panels can be had for ~$80 US and bulk orders greatly reduce that price

- MicroSD: This isn't an innovation, but some new DAPs seem to ignore the standard

- Easily swappable batteries: LiPo cells have great energy density and are cheap to replace. Making batteries easily swappable just improves the end-user experience

- Click wheel interface: Almost no other DAP I've found has a satisfying click wheel interface. The inniosasis Y1 is bearable but doesn't have upgradable storage and the HiFi walker H2 has a jog wheel with separate buttons

- Bluetooth: Yes RockBox devs I hear you, bluetooth will never be supported etc. etc. That isn't in rockbox's scope, I just want to provide support for it through the hardware and an integrated antenna.

- Customisability: Being able to customize things you own is great, and this player was designed with customization in mind. The faceplate, wheel covering, center button and outer housing are all easily replacable and designed to be SLA 3D printed with minimal cost, either by you or a third-party service. The outer shell was designed with sheet metal forming in place and can be made on a press brake.

- Repair: Working in a small space makes the size constraints for this player really tough, so repairability isn't as good as some larger products. In the current edition, the 3.5mm jack and HOLD switch are on a separate daugterboard and designed to be easily replaced (the 3.5mm jack can also be replaced with a 2.5mm or 4.4mm Balanced jack). As mentioned above, the battery and microSD are both also easy to replace and an intelligent BMS using the TP4056 is used to prevent battery damage.
