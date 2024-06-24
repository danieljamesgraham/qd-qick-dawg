# qd-qick-dawg

## Getting Started

Follow qick-dawg [installation guide](https://github.com/sandialabs/qick-dawg/tree/main/installation) until step 3b and connect RFSoC PYNQ to local machine using an Ethernet cable. The LED display on the board should read:

```
RFSoC-PYNQ
No IP detected
```

Set a fixed IP address on the local machine to 192.168.2.1 and set the subnet mask to 255.255.255.0. Use [nmap](https://nmap.org/) to locate the IP address of the dev. board:

```
nmap -sn 192.168.2.1-255
```

Once IP address of board is located, run `nmap 192.168.2.99` (replace default IP address if applicable) to scan and display all open ports. Port 9090 is used to access the board's Jupyter notebook at the address `http://193.168.2.99:9090/lab`.
