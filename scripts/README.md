CWM do-it-all script
=============================

## Installation
```
chmod u+x cwm
sudo ln -s ~/CWM-ProgNets/scripts/cwm /usr/local/bin/cwm
```

## Usage

### Server side
1. Configure required parameters at the top of `cwm`
    - Interface name of source host
    - IP address of source host with netmask
    - IP address of destination host
    - MAC address of destination router/L3 switch/host

2. configure IP address of source host interface
```
cwm ip
```

3. Configure route
```
cwm route
```

4. Configure arp
```
cwm arp
```

5. Configure both route and arp
```
cwm config
```

### Switch side (i.e., Raspberry Pi)
1. Configure required parameters at the top of `cwm`
    - Directory of P4 programs
    - The name of P4 program (without .p4)
    - The name of the first interface
    - The name of the seconf interface

2. Compile P4 program
```
cwm compile
```

3. Run P4 program
```
cwm run
```

4. Compile and run P4 program
```
cwm exec
```

5. Kill running P4 program
```
cwm kill
```

6. Configure table entries with `commands.txt`
```
cwm cli
```


#### Not working? Make sure that the parameters are correct in your script.



