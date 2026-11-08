# openDECTcell

**Free DECT base stations for FRITZ!Box routers running OpenWrt, and a controller that joins them to SIP.**

Many FRITZ!Boxes have a DECT base station built in. Once you install OpenWrt, it goes silent, because its software is part of
AVM's closed firmware. openDECTcell brings it back as free software: register ordinary DECT handsets with the box, connect them
to your SIP account or telephone system, and make HD-voice, encrypted calls, configured in OpenWrt's web interface (LuCI).
Several boxes can act as one DECT network, and handsets roam between them.

> **Experimental software, about 99 % written by AI. No warranty, and not for emergency calls.**
> It already makes real calls on a FRITZ!Box 7520 and 7412 with Gigaset and FRITZ!Fon handsets, but expect rough edges.

## Repositories

| Repository | What it is |
|---|---|
| [**opendectcell**](https://github.com/openDECTcell/opendectcell) | The base station: DECT stack, SIP bridge and the LuCI app, as signed OpenWrt packages. Start here. |
| [**opendectcell-controller**](https://github.com/openDECTcell/opendectcell-controller) | The central controller: handset registry, SIP lines, call log and a web UI, so that many boxes work as one network. Not a PBX. |
| [kmod-lantiq-ssc-pcm](https://github.com/openDECTcell/kmod-lantiq-ssc-pcm) | Kernel driver that runs the Lantiq VR9 SSC as a PCM slave. It carries the voice path of the FRITZ!Box 7412. |
| [kmod-lantiq-tdm-pcm](https://github.com/openDECTcell/kmod-lantiq-tdm-pcm) | Kernel driver for the Lantiq VR9 TDM/PCM block as a PCM slave. It carries the voice path of the FRITZ!Box 7362 SL. |
| [kmod-lantiq-usif-uart](https://github.com/openDECTcell/kmod-lantiq-usif-uart) | Serial driver for the Lantiq VR9 USIF in UART mode. It is the link to the DECT chip on the FRITZ!Box 7362 SL. |

## Get involved

Try it, and tell us which handsets and boxes work for you: see [CONTRIBUTING](https://github.com/openDECTcell/opendectcell/blob/main/CONTRIBUTING.md)
in the main repository. Security problems go through the [security policy](https://github.com/openDECTcell/opendectcell/blob/main/SECURITY.md).
