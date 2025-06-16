---
title: Foxify
author: EndofTimee
description: A portable spotify player that is fox themed
created_at: 2025-6-14
---

I want to make a custom portable music player that had a general fox theme
i would love to try and incorparate somekind of celluar so it can always be used as well as headphone and bluetooth compatiabilty. It of course needs to be able to play spotify songs and i would love if i can make it select playlist you may have! I am also looking at adding in a music player so that you can download songs directly and use that instead of spotify (if you dont have premium or yours songs just arent on spotify)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Currently researching parts
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# Foxify Portable Music Player - Complete Bill of Materials

## Core Processing & Connectivity

| Component | Part Number | Manufacturer | Qty | Unit Cost | Total | Purchase Links | 3D Models | Notes |
|-----------|-------------|--------------|-----|-----------|-------|----------------|-----------|-------|
| **Main MCU Module** | ESP32-S3-WROOM-1-N16R8 | Espressif | 1 | $3.90 | $3.90 | [Digi-Key](https://www.digikey.com/en/products/detail/espressif-systems/ESP32-S3-WROOM-1-N16R8/16162642) • [LCSC $3.75](https://lcsc.com/product-detail/WiFi-Modules_Espressif-Systems-ESP32-S3-WROOM-1-N16R8_C2913202.html) | [SnapEDA](https://www.snapeda.com/parts/ESP32-S3-WROOM-1-N16R8/Espressif%20Systems/view-part/) • [Ultra Librarian](https://app.ultralibrarian.com/details/43a856eb-9b99-11ee-b2d2-0ae0a3b49db5/Espressif-Systems/ESP32-S3-WROOM-1-N16R8) | 16MB Flash, 8MB PSRAM, WiFi/BT |
| **Cellular Module** | EG25-G | Quectel | 1 | $48.00 | $48.00 | [Contact Quectel Direct](https://www.quectel.com/product/lte-eg25-g/) • [FriendlyELEC $45](https://www.friendlyelec.com/index.php?route=product/product&product_id=265) | [Quectel CAD Library](https://www.quectel.com/product/lte-eg25-g/) | **EC25-G discontinued**, EG25-G replacement |
| **SIM Card Connector** | 2174803-2 | TE Connectivity | 1 | $1.95 | $1.95 | [Digi-Key](https://www.digikey.com/en/products/detail/te-connectivity-amp-connectors/2174803-2/5664600) • [Mouser](https://www.mouser.com/ProductDetail/571-2174803-2) | [TE Connectivity CAD](https://www.te.com/usa-en/product-2174803-2.html) | |
| **Cellular Antenna** | FXP73.07.0100A | Taoglas | 1 | $4.04 | $4.04 | [Digi-Key](https://www.digikey.com/product-detail/en/taoglas-limited/FXP73.07.0100A/931-1076-ND/2332703) • [Newark](https://canada.newark.com/taoglas/fxp73-07-0100a/pcb-antenna-2-4835ghz-2-5dbi/dp/72AC5759) | [Octopart](https://octopart.com/fxp73.07.0100a-taoglas-19249590) | Flexible LTE/3G/2G antenna, 100mm |
| **WiFi/BT Antenna** | 2450AT18A100 | Johanson | 1 | $1.20 | $1.20 | [Digi-Key](https://www.digikey.com/en/products/detail/johanson-technology/2450AT18A100/1560836) • [Mouser](https://www.mouser.com/ProductDetail/Johanson-Technology/2450AT18A100) | Johanson CAD Library | 2.4GHz chip antenna |

**Subtotal: $59.09**

## Audio System

| Component | Part Number | Manufacturer | Qty | Unit Cost | Total | Purchase Links | 3D Models | Notes |
|-----------|-------------|--------------|-----|-----------|-------|----------------|-----------|-------|
| **Audio Codec** | WM8960CGEFL/V | Cirrus Logic | 1 | $4.89 | $4.89 | [Octopart Search](https://octopart.com/wm8960cgefl/rv-cirrus+logic-53059078) • [Xecor](https://www.xecor.com/product/wm8960cgefl-rv) | [Ultra Librarian 22+ formats](https://app.ultralibrarian.com/details/43a856eb-9b99-11ee-b2d2-0ae0a3b49db5/Espressif-Systems/ESP32-S3-WROOM-1-N16R8) • [SnapEDA $29](https://www.snapeda.com/) | **V variant replaces discontinued /RV** |
| **Audio Jack** | SJ1-3533NG | CUI Devices | 1 | $1.43 | $1.43 | [Digi-Key](https://www.digikey.com/en/products/detail/cui-devices/SJ1-3533NG/738701) • [Mouser $1.70](https://www.mouser.com/ProductDetail/179-SJ1-3533NG) | [SnapEDA](https://www.snapeda.com/parts/SJ1-3533NG/CUI+Devices/view-part/) • [CUI Official](https://www.cuidevices.com/product/interconnect/connectors/audio-connectors/jacks/sj1-3533ng) | 3.5mm TRRS jack with detection |
| **Speaker** | CSS-40408N | CUI Devices | 1 | $4.25 | $4.25 | [SameSky $4.25](https://www.sameskydevices.com/product/audio/speakers/miniature-(10-mm~40-mm)/css-40408n) • [RS Components](https://in.rsdelivers.com/product/cui-devices/cds-40288/cui-devices-6w-miniature-speaker-40mm-lead-length/2596138P) | [SameSky CAD Library](https://www.sameskydevices.com/product/audio/speakers/miniature-(10-mm~40-mm)/css-40408n) | |
| **Audio Capacitors** | Various | Murata/TDK | 8 | $0.15 | $1.20 | [Digi-Key Caps](https://www.digikey.com/en/products/filter/ceramic-capacitors/60) • [LCSC Bulk](https://lcsc.com/products/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_1649.html) | Standard footprints | Low-ESR caps for audio filtering |
| **Ferrite Bead** | | | | | | | | Audio isolation |

**Subtotal: $11.77**

## Display & User Interface

| Component | Part Number | Manufacturer | Qty | Unit Cost | Total | Purchase Links | 3D Models | Notes |
|-----------|-------------|--------------|-----|-----------|-------|----------------|-----------|-------|
| **LCD Display** | | |||||||
| **Touch Controller** | FT6236 | FocalTech | 1 | $2.50 | $2.50 | [Datasheet4U](https://datasheet4u.com/datasheet-pdf/FocalTechSystems/FT6236/pdf.php?id=958370) • Contact Asian suppliers | Limited CAD availability | **Typically integrated in display modules** |
| **Display Connector** | FH12-24S-0.5SH(55) | Hirose | 1 | $1.68 | $1.68 | [Digi-Key](https://www.digikey.com/en/products/detail/hirose-electric-co-ltd/FH12-24S-0-5SH-55/1110322) • [Mouser](https://www.mouser.com/ProductDetail/Hirose-Electric/FH12-24S-0.5SH55) | [Hirose Official CAD](https://www.hirose.com/product/series/FH12) • [SamacSys](https://www.samacsys.com/category/3d-models/) | **Updated part - (55) variant** |
| **Touch Connector** | FH12-6S-0.5SH(55) | Hirose | 1 | $1.45 | $1.45 | [Digi-Key](https://www.digikey.com/en/products/detail/hirose-electric-co-ltd/FH12-10S-0.5SH-55/1110372) • [Octopart](https://octopart.com/fh12-6s-0.5sh(55)-hirose-39503285) | [Hirose Official CAD](https://www.hirose.com/product/series/FH12) | 6-pin 0.5mm FPC connector |
| **Tactile Buttons** | SKHHPKA010 | Alps | 4 | $0.95 | $3.80 | [Chip1Stop](https://www.chip1stop.com/USA/en/product/detail?partId=ALPS-0000143) • LCSC for volume | Alps CAD Library | Play/pause, prev, next, power |
| **Rotary Encoder** | PEC11R-4220F-S0024 | Bourns | 1 | $8.20 | $8.20 | [RS Components](https://uk.rs-online.com/web/p/mechanical-rotary-encoders/7377767) • [Digi-Key](https://www.digikey.com/en/products/detail/bourns-inc/PEC11R-4220F-S0024/1088313) | [Bourns Official](https://www.bourns.com/products/encoders/optical-encoders) | 24-pulse rotary encoder |

**Subtotal: $17.63** *
## Power Management & Battery

| Component | Part Number | Manufacturer | Qty | Unit Cost | Total | Purchase Links | 3D Models | Notes |
|-----------|-------------|--------------|-----|-----------|-------|----------------|-----------|-------|
| **USB-C PD Controller** | IP5328P | Injoinic | 1 | $0.86 | $0.86 | [LCSC 4,780 stock](https://lcsc.com/product-detail/Others_IP5328P_C188809.html) • [Abra Electronics](https://abra-electronics.com/batteries-holders/battery-chargers-testers/xl-7001-ip5328p-3.7v-to-5v-9v-12v-step-up-fast-quick-charger-circuit-board-qc2.0-qc3.0.html) | [SnapEDA](https://www.snapeda.com/parts/IP5328P/Injoinic/view-part/) • [Datasheet4U](https://datasheet4u.com/datasheet/Injoinic/IP5328P-1261761) | Bidirectional USB-C up to 22.5W |
| **Battery** | 
| **USB-C Connector** | USB4105-GF-A-060 | Global Connector | 1 | $0.69 | $0.69 | [LCSC](https://lcsc.com/product-detail/usb-connectors_global-connector-technology-usb4105-gf-a-060_C3025063.html) • [Newark $1.89](https://www.newark.com/gct-global-connector-technology/usb4105-gf-a/usb-conn-2-0-type-c-rcpt-16pos/dp/86AH2021) | [SnapEDA](https://www.snapeda.com/parts/USB4105-GF-A/Global%20Connector%20Technology/view-part/) | USB-C receptacle, 5A/240W rating |
| **Fuel Gauge IC** | MAX17048G+T10 | Analog Devices | 1 | $2.01 | $2.01 | [Digi-Key](https://www.digikey.com/en/products/detail/maxim-integrated/MAX17048G-T10/3758921) • [Mouser 23k+ stock](https://www.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/MAX17048G+T10?qs=D7PJwyCwLAoGnnn8jEPRBQ%3D%3D) | [SnapEDA](https://www.snapeda.com/parts/MAX17048G+T10/Analog%20Devices/view-part/) • [Analog Official](https://www.analog.com/en/products/max17048.html) | Battery capacity monitoring |
| **Protection IC** | ||||||| Battery protection |
| **Power MOSFET** | AO3401A | Alpha & Omega | 2 | $0.44 | $0.88 | [Digi-Key](https://www.digikey.com/en/products/detail/alpha-omega-semiconductor-inc/AO3401A/1855773) • [LCSC bulk pricing](https://lcsc.com/product-detail/MOSFETs_Alpha-Omega-Semicon-AO3401A_C15127.html) | [SnapEDA](https://www.snapeda.com/) | P-channel 30V 4A protection switches |
| **Charging LED** | LTST-C19HE1WT | Lite-On | 4 | $0.12 | $0.48 | [Mouser 682k+ stock](https://www.mouser.com/ProductDetail/Lite-On/LTST-C19HE1WT) • [Digi-Key](https://www.digikey.com/en/products/detail/lite-on-inc/LTST-C19HE1WT/2208082) | Standard 0606 footprint | RGB battery level indicators |
| **Power Switch** | EG1218 | E-Switch | 1 | $0.95 | $0.95 | [Digi-Key](https://www.digikey.com/en/products/detail/e-switch/EG1218/101726) • [Mouser](https://www.mouser.com/ProductDetail/E-Switch/EG1218) | [SnapMagic](https://insights.snapmagic.com/syndication) • [Ultra Librarian](https://app.ultralibrarian.com/) | Main power slide switch |

**Subtotal: $5.96**

## Passive Components & Power

| Component | Part Number | Manufacturer | Qty | Unit Cost | Total | Description |
|-----------|-------------|--------------|-----|-----------|-------|-------------|
| **Capacitors 0805** | Various | Murata/Samsung | 50 | $0.08 | $4.00 | 0.1µF, 1µF, 10µF, 22µF |
| **Capacitors 1206** | Various | Murata/Samsung | 10 | $0.25 | $2.50 | 47µF, 100µF tantalum |
| **Resistors 0603** | Various | Yageo/Vishay | 40 | $0.03 | $1.20 | Various values |
| **Inductors** | Various | Murata/TDK | 6 | $0.35 | $2.10 | Power supply filtering |
| **Crystal** | NX5032GA-12.000000MHZ | NDK | 1 | $0.85 | $0.85 | 12MHz crystal for ESP32 |
| **LDO Regulators** | AP2112K-3.3TRG1 | Diodes Inc | 2 | $0.35 | $0.70 | 3.3V rails |

**Subtotal: $11.35**


## Mechanical & Enclosure

| Component | Part Number | Manufacturer | Qty | Unit Cost | Total | Description |
|-----------|-------------|--------------|-----|-----------|-------|-------------|
| **Gaskets** | Various | Custom | 4 | $0.50 | $2.00 | Sealing gaskets |
| **Screws** | M2.5×8mm | Various | 8 | $0.10 | $0.80 | Case assembly screws |
| **Standoffs** | Various | Keystone | 6 | $0.25 | $1.50 | PCB mounting standoffs |

**Subtotal: $4.30**

--

### **Total BOM Cost: $110.10**

~~~~~~~~~~~~~~
still need battery & lcd
have spent ~3 hours researching parts
~~~~~~~~~~~~~~
