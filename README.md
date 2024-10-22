# ZenStates-Linux
Collection of utilities for Ryzen processors and motherboards

## zenstates.py
Dynamically edit AMD Ryzen processor P-States

Requires root access and the msr kernel module loaded (just run "modprobe msr" as root).

    usage: zenstates.py [-h] [-l] [-p {0,1,2,3,4,5,6,7}] [--enable] [--disable]
                        [-f FID] [-d DID] [-v VID] [--c6-enable] [--c6-disable]
                        [--cpb-enable] [--cpb-disable]
    
    Sets P-States for Ryzen processors
    
    options:
      -h, --help            show this help message and exit
      -l, --list            List all P-States
      -p {0,1,2,3,4,5,6,7}, --pstate {0,1,2,3,4,5,6,7}
                            P-State to set
      --enable              Enable P-State
      --disable             Disable P-State
      -f FID, --fid FID     FID to set (in hex)
      -d DID, --did DID     DID to set (in hex)
      -v VID, --vid VID     VID to set (in hex)
      --c6-enable           Enable C-State C6
      --c6-disable          Disable C-State C6
      --cpb-enable          Enable Core Performance Boost
      --cpb-disable         Disable Core Performance Boost
