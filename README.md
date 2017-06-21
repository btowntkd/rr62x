# RocketRaid 62x Linux Drivers
- DKMS instructions were taken from https://help.ubuntu.com/community/RocketRaid
- Updated module source was forked from https://github.com/clockfort/rr62x

# Instructions
1. Clone the module source code and dkms config file directly into the appropriate /usr/src directory (expected by DKMS):
    - 'sudo git clone https://github.com/btowntkd/rr62x.git /usr/src/rr62x-1.2'
2. Add the DKMS module:
    - 'sudo dkms add -m rr62x -v 1.2'
3. Build the DKMS module:
    - 'sudo dkms build -m rr62x -v 1.2'
4. Install the module:
    - 'sudo dkms install -m rr62x -v 1.2'
5. Probe for the newly-usable hardware:
    - 'sudo modprobe rr62x'

## TL;DR
Copy and paste this block into your terminal, and press enter.
```
sudo git clone https://github.com/btowntkd/rr62x.git /usr/src/rr62x-1.2
sudo dkms add -m rr62x -v 1.2
sudo dkms build -m rr62x -v 1.2
sudo dkms install -m rr62x -v 1.2
sudo modprobe rr62x
```
