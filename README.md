# Subtext Integrations
Here you will find instructions and examples for getting Subtext up and running with different media servers. 
Subtext is built to be flexible, modular and able to work with every media server on the market, as well as with 
custom solutions created by users and developers.

This repository contains everything you need to get Subtext up and running with your system.

More information about Subtext can be found at www.subtxt.io.

## Protocols
Subtext is built to listen for commands on a variety of protocols, depending on the system presenting the media for 
subtitle synchronization. It uses a set of modules, "timecode providers," to accept individual protocols. Currently, 
there are:
* OSC
* TCP
* UDP
* LTC
* HTTP
* Autosync (coming soon)

Each of these accepts an identical set of commands for controlling timecode being sent to users' devices. They can 
be enabled and disabled on a node using environment variables on the Balena dashboard.
### Absolute vs Freerun
Subtext nodes are intended to operate in one of two modes, absolute or freerunning timecode. **Absolute** timecode 
accepts messages from the media server containing a specific time.
**Freerunning** 
timecode expects start and stop commands from the media server and generates timecode on the device.

NightLight Labs recommends absolute timecode for the most accuracy.

## Media Server Examples
In this repository, there are a number of examples for how to send control messages from various media servers. This 
is not meant as an exhaustive list, and there are almost certainly other ways for the servers in these examples to 
provide timecode. These examples are meant as starting points and suggestions for getting your setup up and running.

All of the examples presuppose a working konwledge of the server being demonstrated.