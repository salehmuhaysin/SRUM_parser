# SRUM_parser
Parse Windows System Resource Usage Monitor (SRUM)  
SRUM used by Windows Operating System to monitor utilization usage of the resources (Network connections, Application running, energy usage, etc.)

to read more about SRUM, [click here](https://github.com/libyal/esedb-kb/blob/master/documentation/System%20Resource%20Usage%20Monitor%20(SRUM).asciidoc)

### Usage:
![alt text](https://github.com/salehmuhaysin/SRUM_parser/blob/master/Selection_005.png?raw=true)

#### Arguments:

```
required arguments:  
  -i IN_FILE      Input path for SRUDB.dat file  
  -o OUT_FILE     Output path (srum.csv) will output folder as srum-[srum_type].csv  
  
optional arguments:  
  -h, --help      show this help message and exit  
  -r RESULT_TYPE  Result files (json, csv), by default output in csv file  
```


### Output

The results either csv or json format (identified by arg **-r**) written to files (identified by arg **-o**).  
Output files: 

Data Type         | Output File
----------------- | ----------------
ApplicationResourceUsage | _<output_file>_-ApplicationResourceUsage.csv
NetworkConnectivityUsageMonitor | _<output_file>_-NetworkConnectivityUsageMonitor.csv
NetworkDataUsageMonitor | _<output_file>_-NetworkDataUsageMonitor.csv


### Requirements

> sudo apt-get install python-libesedb


