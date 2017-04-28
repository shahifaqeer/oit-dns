# DNS Data Analysis



### Data Extraction

* Follow the instructions at https://goo.gl/3cSlxI to start your `Spark` setup over `NS cluster`.

* Clone the ```oit-dns``` repository from Github:
```bash 
$ git clone https://github.com/shahifaqeer/oit-dns.git
```

* Change the directory:
```bash
$ cd oit-dns
```

* All data files are available at `/tigress/arpitg`. The path for consolidated logs is: 
`/tigress/arpitg/dns_data/tshark_20170207_20170212_consolidated`

* Each line in the consolidated logs is of the form:
```
timestamp, XX, srcIP, dstIP, qname, qtype, macAddr, subnet, host_type, 
host_name, system_type, OS, nic_manufacturer
```
Example:
```
1486868340.927547000,0.039027000,10.9.74.206,10.8.0.5,as-sec.casalemedia.com,0x00000001,
C4:B3:01:CC:6E:CB,vapornet100,host-dynamic,nat-oitwireless-inside-vapornet100-c-19150,,,Apple
```

* Scripts that join multiple data sets to generate the consolidated logs are in the 
directory: `data_extraction` 

### Feature Extraction

* Add your scripts to the  `feature_extraction` directory. 

* ...

