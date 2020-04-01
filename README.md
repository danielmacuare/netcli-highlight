# netcli-highlight
**TLDR:** The repo will show you how to use syntax highlighting on Live Network Devices. (Juniper/Cisco/Arista)


## TOC
* [What's this about?](#what's-this-about?)
* [Use-Cases](#use-cases)
* [Benefits](#benefits)
* [Pre-requisites](#pre-requisites)
* [Usage](#usage)
* [Purpose](#purpose)
* [Limitations](#limitations)
* [Thanks](#thanks)



## What's this about?
If you have ever used the CLI on network devices, you probably have ended up frustrated trying to make sense of the long lines of configuration. Although nowadays the use of editors like `Sublime/Vscode/Atmom` can provide some really useful syntax highlighting, you still can find yourself struggling to read the config files or outputs while you are on live devices.

<br/>

**Here we have a Juniper SRX firewall policy.** This rule is comprised by source/destination/application/actions, if you need to read one of them it's alright but if your output has you reading over 10 rules you can see how difficult is to differentiate each component.

![Junos FW Rule](resources/Junos_Sec_Pol.png)

**Wouldn't be nice to have some live syntax highlight to differentiate each component and quickly find what you are looking for?** Something like...

![Junos Colored FW Rule](resources/Junos_Sec_Pol-Colored.png)

If you are like me, fascinated by the concept of `marginal gains`, this will config will help you to read config files and output quicker, and in general to work more efficiently in the CLI.

The purpose of this repo is to give you an idea of the power of having a syntax highlighting **while working on live devices**.

**Note: The default color code has been tested using a Dark terminal Background as you can see in the images above**

## Use-cases
- Reading Firewall Rules (JunOS)
- Reading show ip bgp summary (Cisco / Arista)
![Show ip bgp summary](resources/show_ip_bgp_summary.png)

- Reading show interfaces (Cisco / Arista / JunOS)
![Show interfaces](resources/show_int.png)

- 


## Benefits
- Quicker troubleshooting as you can easily identify missconfigurations or things like interfaces down.
-  
- Color codes can be totally customised to your liking. To see the available HTML color codes go [HERE](https://htmlcolorcodes.com/)
- Regex canbe customised to adapt it to  your particular Network OS (NOS) and version.


## Pre-requisites
 - Python 3.6+
 - [Chromaterm](https://github.com/hSaria/ChromaTerm) - A big shout out to **hSaria** for buliding this wonderful too.


## Usage




## Limitations
- There are countless of NOS and versions so not all of them would probably work with [this config file](.chromaterm.yml) but you can easily modify it to filter the content you consider important and even customise the colors to your liking.
- [This config file](.chromaterm.yml) has been tested with a limited amount of Juniper, Cisco and Arista devices.

## Thanks
Thanks to [hSaria](https://github.com/hSaria) for creating this fantastic tool [Chromaterm](https://github.com/hSaria/ChromaTerm)