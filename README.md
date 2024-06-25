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

Once IP address of board is located, run `nmap 192.168.2.99` (replace default IP address if applicable) to scan and display all open ports. Port 9090 is used to access the board's Jupyter notebooks at the address `http://193.168.2.99:9090/lab`.

Install the necessary files from the quick-dawg package onto the FPGA. The password required when prompted is `xilinx`. Run the following commands when in the `qick-dawg` directory:

```
scp -r installation xilinx@192.168.2.99:/home/xilinx/jupyter_notebooks
scp -r qick xilinx@192.168.2.99:/home/xilinx/jupyter_notebooks
```

Run all the cells in `installation/Install_Packages_LAN.ipynb` to complete the installation of the necessary packages. Resume the installation guide at step 3d.
