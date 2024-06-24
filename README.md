# qd-qick-dawg

## Getting Started

Follow qick-dawg [installation guide](https://github.com/sandialabs/qick-dawg/tree/main/installation) up to step 3b and connect RFSoC PYNQ to local machine using an Ethernet cable. The display on the board should display:

```
RFSoC-PYNQ
No IP detected
```

Set fixed IP address on local machine to 192.168.2.1 and set subnet mask to 255.255.255.0.Use [nmap](https://nmap.org/) to locate IP address of dev. board:

```
nmap -sn 192.168.2.1-255
```
