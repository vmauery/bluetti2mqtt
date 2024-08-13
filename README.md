# Bluetti2MQTT

![update-badge](https://img.shields.io/github/last-commit/vmauery/bluetti2mqtt?label=Last%20Updated)

## Installation
To add this repository to Home Assistant use the badge below:

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fvmauery%2Fbluetti2mqtt)

or add it manually by navigating to `Settings` > `Add-ons` > `Add-on Store`

Select the three dot menu in the upper right, choose `Repositories`, and add the following url:
```
https://github.com/vmauery/bluetti2mqtt
```

Refresh the page (hard refresh may be required), scroll down to Bluetti2MQTT and install the add-on.

## Add-ons

This repository contains the following add-ons:

### [Bluetti2MQTT](./bluetti2mqtt)

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]
![Supports i386 Architecture][i386-shield]

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-shield]: https://img.shields.io/badge/i386-yes-green.svg

_MQTT bridge between Bluetti and Home Assistant._

This is a fork from https://github.com/ftrueck/bluetti2mqtt which is a
fork from https://github.com/SSMCD/bluetti2mqtt

The original SSMCD code pulls in bluetti-mqtt from pip, which is an
old version. Even the latest https://github.com/warhammerkid/bluetti_mqtt
code does not support the AC70. But the https://github.com/ftrueck/bluetti_mqtt
fork does contain support for it. So what MY fork of bluetti2mqtt does
is pull the bluetti-mqtt from the ftruek fork correctly, since there were
some issues the in ftrueck dockerfile for bluetti2mqtt. But when I add this
repo to HA, I can see my device.
