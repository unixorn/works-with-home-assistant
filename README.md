# works-with-home-assistant

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Table of Contents

- [Hubs](#hubs)
- [Wifi devices](#wifi-devices)
- [Zigbee](#zigbee)
- [Z-Wave](#z-wave)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

This is a list of stuff that works with Home Assistant with minimal aggravation.

If you have to reflash the device, please add that to the **Notes** column. If you need to add a plugin to HAss before it can be used, add that to **Notes** too.

## Hubs

| Name   | Description                                      | Notes           |
| ------ | ------------------------------------------------ | --------------- |
| [GoControl CECOMINOD016164 HUSBZB-1 USB Hub](https://smile.amazon.com/gp/product/B01GJ826F8) | USB device with both Z-Wave and Zigbee radios. ||

## Wifi devices

If items here need reflashing to work with Home Assistant, please state that in the **Notes** column.

| Name   | Description                                      | Notes           |
| ------ | ------------------------------------------------ | --------------- |

## Zigbee

| Name   | Description                                      | Notes           |
| ------ | ------------------------------------------------ | --------------- |
| [GE 45856GE Zigbee Smart Switch In-Wall Lighting Control](https://smile.amazon.com/gp/product/B019HTH2A0/) | In-wall switch | Requires a neutral wire |
| [Samsung SmartThings Motion Sensor](https://smile.amazon.com/gp/product/B01IE35PCC) | Detects temperature and motion ||
| [Securifi Peanut Smart Plug](https://smile.amazon.com/gp/product/B00TC9NC82) | Small cheap smart plug with power switch. Monitors the energy consumption of the plugged-in device.  ||

## Z-Wave

A note on dimmers: Lutron holds a patent for sending status back to hubs on their RadioRA2 system. Not all zwave dimmers license this patent, so some act weird. Leviton is known to license this patent, and their dimmers work well.

| Name   | Description                                      | Notes           |
| ------ | ------------------------------------------------ | --------------- |
| [Aeotec Range Extender 6, Z-Wave Plus repeater](https://smile.amazon.com/gp/product/B01M6CKJXC) | Range extender for Z-Wave. | While it works, it's probably more useful to just buy a Z-Wave smart plug than to get a dedicated  range extender |
| [Aeotec Smart Outlet](https://smile.amazon.com/gp/product/B07PJNL5DB/) | 15 Amp. Monitors electricity usage as well as controlling a device ||
| [GE Enbrighten Z-Wave Plus Smart Plug](https://smile.amazon.com/gp/product/B06W9NWFM3) | Outdoor rated, also works as a range extender. ||
| [GE/Jasco Decora Smart Switch](https://smile.amazon.com/GE-Repeater-Extender-SmartThings-14291/dp/B01M1AHC3R/) | Wall Switch. 3 Way compatible, but will require an add-on switch, and supports up to four ||
| [Leviton DD00R-DLZ 120VAC 60 Hz Decora Digital/Decora Smart Matching Dimmer Remote](https://smile.amazon.com/gp/product/B01AFU1KOY) | Remote for the [DZ6HD-1BZ Dimmer](https://smile.amazon.com/gp/product/B01N4F487U) ||
| [Leviton DZ6HD-1BZ Dimmer](https://smile.amazon.com/gp/product/B01N4F487U) | Dimmer - 600  Watt incandescent or 300W LED or CFL. Requires a neutral wire. ||
