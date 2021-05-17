# Simple file storage for Libre Solar device information

The folder `files` of this repository is deployed to [files.libre.solar](https://files.libre.solar) after each push.

The information provided by ThingSet is not sufficient to create a nice user interface, so it should be enhanced with extra information. This sort of extra information will not be stored on the device, but on a file server, which can also store the device manual, firmware upgrades, etc.

Below are some *preliminary* suggestions for the file system structure.

## User Manual

Example path: `https://files.libre.solar/manuals/mppt-1210-hus-0v3-en.pdf`

Two-letter language tag at the end according to [ISO 639-1](https://en.wikipedia.org/wiki/ISO_639-1).

## Firmware binaries

Example path: `https://files.libre.solar/fw/charge-controller/v20.0/mppt-1210-hus.bin`

Possible alternative: MCUboot image format

Extra information stored in JSON file together with firmware.

## JSON firmware info file

Example path: `https://files.libre.solar/fw/charge-controller/v20.0/thingset-info.json`
