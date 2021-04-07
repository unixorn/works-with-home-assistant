<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Table of Contents

- [works-with-home-assistant](#works-with-home-assistant)
  - [Introduction](#introduction)
    - [Things to think about before picking a platform](#things-to-think-about-before-picking-a-platform)
    - [A note on dimmers](#a-note-on-dimmers)
    - [Stuff that _doesn't_ work](#stuff-that-_doesnt_-work)
  - [Hubs](#hubs)
  - [Wifi devices](#wifi-devices)
  - [Zigbee](#zigbee)
  - [Z-Wave](#z-wave)
  - [Non-working devices](#non-working-devices)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->
# works-with-home-assistant

[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Funixorn%2Fworks-with-home-assistant%2Fbadge%3Fref%3Dmain&style=flat)](https://actions-badge.atrox.dev/unixorn/works-with-home-assistant/goto?ref=main)
[![GitHub stars](https://img.shields.io/github/stars/unixorn/works-with-home-assistant.svg)](https://github.com/unixorn/works-with-home-assistant/stargazers)
[![GitHub last commit (branch)](https://img.shields.io/github/last-commit/unixorn/works-with-home-assistant/main.svg)](https://github.com/unixorn/works-with-home-assistant)

## Introduction

This is a list of devices that work with Home Assistant with minimal aggravation.

If you have to reflash a device, please add that to the **Notes** column.

If you need to add a plugin to Home Assistant before it can be used, add that to **Notes** too.

If it requires the devices connect to an internet server, even just for initial configuration, please add that to **Notes** - I want it easy to see which devices won't brick if the vendor goes out of business and also aren't vulnerable to some jackass hacking the company's servers.

### Things to think about before picking a platform

Read [Zigbee and WIFI Cooexistence](https://www.metageek.com/training/resources/zigbee-wifi-coexistence.html) on Metageek for more details, but Zigbee can interfere with 2.4GHz WIFI, Z-Wave doesn't. And since a lot of WIFI IOT gear seems to only work on 2.4GHz, you may want to go Z-Wave if you're just starting to buy equipment.

### A note on dimmers

Lutron holds a patent for sending status back to hubs on their RadioRA2 system. Not all Z-Wave or Zigbee dimmers license this patent, so some act weird. Leviton is known to license this patent, and their dimmers work well.

### Stuff that _doesn't_ work

It's ok to add entries for things that didn't work, but be very clear in the notes field that it didn't work & why it didn't work so people can be warned and not waste money on devices which won't work with HA.
## Hubs

| Name   | Description                                      | Notes           |
| ------ | ------------------------------------------------ | --------------- |
| [GoControl CECOMINOD016164 HUSBZB-1 USB Hub](https://smile.amazon.com/gp/product/B01GJ826F8) | USB device with both Z-Wave and Zigbee radios. ||

## Wifi devices

If items here need reflashing to work with Home Assistant, please state that in the **Notes** column.

| Name   | Description                                      | Notes           |
| ------ | ------------------------------------------------ | --------------- |
| [OpenGarage.io garage door opener/sensor](https://opengarage.io) | Combination garage door opener and sensor | This is very nice piece of hardware. Completely configurable through it's web interface. In addition to being usable with Blynk and IFTTT, it also has a dedicated cross-platform app, and more interestingly, a well described REST api and can send MQTT messages for ingestion by Home Assistant. And the firmware is on Github, if you want to modify it. |

## Zigbee

| Name   | Description                                      | Notes           |
| ------ | ------------------------------------------------ | --------------- |
| [Aqara Vibration Sensor](https://smile.amazon.com/gp/product/B07PJT939B) | Mini glass break detector | This was a pita to add to my HA. Once your HA is scanning for new devices, press and hold the button on the sensor for ~5 seconds until the lights flash, then you have to press it again (but don't hold it, press and release) every second or two until HA finds it. At least it is cheap. |
| [Aqara Water Leak Sensor](https://smile.amazon.com/gp/product/B07D39MSZS) | Water leak detector | The manual was unclear on how to put it in pairing mode - press the water droplet icon firmly until the hidden light flashes three times, then let go.<p>These also ship ready to go - no messing with the battery, just press the button and you can add it to your Zigbee mesh. Edit after 2 months - this keeps dropping off my zigbee mesh and I don't recommend it. |
| [GE 45856GE Zigbee Smart Switch In-Wall Lighting Control](https://smile.amazon.com/gp/product/B019HTH2A0/) | In-wall switch. | Requires a neutral wire. ||
| [Samsung SmartThings Motion Sensor](https://smile.amazon.com/gp/product/B01IE35PCC) | Detects temperature and motion. ||
| [Samsung SmartThings Water Sensor](https://smile.amazon.com/gp/product/B07F951JDP) | A cheap small water sensor. Reports wet/dry status for the zone. ||
| [Securifi Peanut Smart Plug](https://smile.amazon.com/gp/product/B00TC9NC82) | Small cheap smart plug with controllable power switch. | Reliable cheap smart plug. Claims to also monitor the energy consumption of the plugged-in device, but monitoring doesn't work. |

## Z-Wave

| Name   | Description                                      | Notes           |
| ------ | ------------------------------------------------ | --------------- |
| [Aeotec Range Extender 6, Z-Wave Plus repeater](https://smile.amazon.com/gp/product/B01M6CKJXC) | Range extender for Z-Wave. | While it works, it's probably more useful to just buy a Z-Wave smart plug than to get a dedicated range extender. |
| [Aeotec Smart Outlet](https://smile.amazon.com/gp/product/B07PJNL5DB/) | 15 Amp. Monitors electricity usage as well as controlling a device. ||
| [Dome Leak Sensor](https://smile.amazon.com/gp/product/B01LXR0B8Q/) | Water leak sensor. Reports via Z-Wave when water is detected and also has an audible alarm. | I like that it comes with a four foot sensor probe so you can use it in a sump or other awkward location. |
| [GE Enbrighten Plug in Z-Wave Smart Switch](https://smile.amazon.com/gp/product/B004AMB3CI/) | Plug-in Single Outlet with button. ||
| [GE Enbrighten Z-Wave Plus Smart Plug](https://smile.amazon.com/gp/product/B06W9NWFM3) | Outdoor rated, also works as a range extender. ||
| [GE/Jasco Decora Smart Switch](https://smile.amazon.com/gp/product/B01M1AHC3R/) | Wall Switch. 3 Way compatible.| Requires an add-on remote switch to work with 3 way. Supports up to four add-on switches. |
| [GE/Jasco Standard Smart Switch](https://smile.amazon.com/gp/product/B07X6JW72G/) | Wall Switch. 3 Way compatible.| Requires an add-on remote switch to work with 3 way. Supports up to four add-on switches. |
| [Inovelli Black Series Dimmer](https://smile.amazon.com/gp/product/B07RYMSH6Q) | Wall Switch. 3 Way compatible. Dimmer| No Neutral required, but recommended. Depending on zwave integraton, may need special setup (https://support.inovelli.com/portal/en/kb/inovelli/switches) |
| [Inovelli Black Series On/Off](https://smile.amazon.com/gp/product/B07T2416D8) | Wall Switch. 3 Way compatible.| No Neutral required, but recommended. Depending on zwave integraton, may need special setup (https://support.inovelli.com/portal/en/kb/inovelli/switches) |
| [Inovelli Red Series Dimmer](https://smile.amazon.com/gp/product/B07S1BMMGH) | Wall Switch. 3 Way compatible. Dimmer| No Neutral required, but recommended. Depending on zwave integraton, may need special setup (https://support.inovelli.com/portal/en/kb/inovelli/switches) Energy Monitoring, Scene Control, RGB Notifications|
| [Inovelli Red Series On/Off](https://smile.amazon.com/gp/product/B07T26MVYC) | Wall Switch. 3 Way compatible.| No Neutral required, but recommended. Depending on zwave integraton, may need special setup (https://support.inovelli.com/portal/en/kb/inovelli/switches) Energy Monitoring, Scene Control, RGB Notifications|
| [Leviton DD00R-DLZ 120VAC 60 Hz Decora Digital/Decora Smart Matching Dimmer Remote](https://smile.amazon.com/gp/product/B01AFU1KOY) | Remote in-wall switch for the [DZ6HD-1BZ Dimmer](https://smile.amazon.com/gp/product/B01N4F487U). ||
| [Leviton DZ6HD-1BZ Dimmer](https://smile.amazon.com/gp/product/B01N4F487U) | Dimmer - 600 Watt incandescent or 300W LED or CFL. Requires a neutral wire. | Periodically (roughly every three to six months) I've run into issues where it locks up with the lights stuck on, but if you trigger the airgap functionality (pull the dimmer lever gently till it clicks and the light on the switch goes out, wait five seconds and push it back into place) it reboots and starts working again. |
| [Monoprice Z-Wave Plus Smart Plug](https://www.monoprice.com/product?p_id=27481) | Smart Plug | A good lower-priced alternative to the Aeotec Smart Outlet. Monitors power usage and voltage. Extremely easy to pair with Home Assistant. |
| [ZOOZ Z-Wave Plus 4-in-1 Sensor ZSE40](https://smile.amazon.com/gp/product/B01AKSO80O/) | Motion, light, temperature, and humidity sensor. | Quirky little device. It measures light on a scale of 0-100%, and not lux. It requires a [templated `binary_sensor`](https://www.home-assistant.io/docs/z-wave/entities/#burglar-entity) to make the burglar sensor work as a motion sensor in Home Assistant. |

## Non-working devices

This section is for things that you've tried and did not get to work with HA.

| Name   | Description                                      | Notes           |
| ------ | ------------------------------------------------ | --------------- |
