# !!! This is still a work in progress !!!
Documentation is not reviewd.
Energy consumption differs from the app but maybe in a good way? Closer to grid provider.

An *easy-to-use YAML-based integration* for Sigenergy inverters, battery and DC charger for Home Assistant. 

# Contents
- [1. Overview](#1-overview)
- [2. Documentation](#2-documentation)
    - [Installation/ Configuration](wiki/FAQ:-How-to-install)
    - [Dashboard Setup](wiki/How-to-configure-the-dashboards)
    - [Usage Instructions](wiki/FAQ:-How-to-use)
    - [FAQ, Troubleshooting, Known Issues](wiki/FAQ:-Problems-with-the-connection)
    - [Roadmap](doc/issues_roadmap.md)
- [3. Support](#3-support)
- [4. Visual impressions](#4-visual-impressions)
- [5. Tested configurations](#5-tested-configurations)
- [6. Status and future work](#6-status-and-future-work)
- [7. Contribution](#7-contribution)


# 1. Overview

This integration lets you gather sensor data and control the EMS (Energy Management System) of Sigenergy inverter, battery and DC charger.

## 2. Documentation

The documentation covers following topics:

[Installation/ Configuration](wiki/FAQ:-How-to-install)

[Dashboard Setup](wiki/How-to-configure-the-dashboards)

[Usage Instructions](wiki/FAQ:-How-to-use)

[Wiki: FAQ, Troubleshooting, Known Issues](wiki/)

## 3. Support

If you any kind of assistance, you have three options:

a) Use the [github discussion](../../discussions) 

b) Only if code-related (bugs / contributions): Open an  [github issue](../../issue) or isse a pullrequest

## 4. Visual impressions

Home Asisstants built-in Energy Dashboard

<img src="doc/images/HA_Energy_Dashboard.png" width="600">


Default dashboard tab "overview"

<img src="doc/images/Dashboard_Overview.png" width="600">


Default dashboard tab "Detail"

<img src="doc/images/Dashboard_Detail.png" width="600">


Default dashboard tab "EMS"

<img src="doc/images/Dashboard_EMS.png" width="600">


## 5. Tested configurations
I have a **Sigenergy SigenStor EC 15.0 TP** Inverter and **2 8kWh batteries** updating frequently to the latest **Home Assistant** (> 2023.3). I try to thoroughly test features before releasing them, but I cannot test everything (e.g., backup capabilities, DO-related, ...)

The Modbus register mapping is based on two documents I found online. I am not sure if I am allowed to share the files, but you can search for them using their names. 
Let me know in the github discussions, if there are newer versions available.

```
Sigenergy Modbus Protocol
Version: V1.7
Release date: 2024-04-09
483828-sigenergy-modbus-protocol-20240409-pdf
```

## 6. Status and future work 
1. ReadOnly parameters are read.
2. 


## 7. Contribution
We are happy to share our experiences - feel encouraged to share yours with us, too! 

If you have any questions, feature requests, found any bugs or have some hints how to update the documentation, just ask on Github Discutions.

**Thanks to all the people, who are actively contributing to this project! Special thanks to @mkaiser for the Sungrow integration on wich this is based**
