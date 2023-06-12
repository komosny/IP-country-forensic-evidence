# Country location evidence from IP address

Raw data and source code for the paper [Evidential value of country location evidence obtained from IP address geolocation](https://peerj.com/articles/cs-1305/).

# Content

## Directories

- atlas - daily operational reports of Atlas devices 2015 to 2022 (raw data)
- figures - generated plots for the commercial geolocation database IP2Location DB1
- geodata - free geolocation database IP2Location DB1 LITE
- geography - country border maps
- history - compiled historical dataset
- maps - Atlas coverage maps in countries
- precomp - precomputed historical dataset

## Files
- notebook.inbp - notebook with source code
- enviroment.txt - python and module versions

# Reproducibility
The notebook reproduces the results for the free geolocation database.

## Database license

The notebook works by default with the free version of the geolocation database. The commercial version cannot be distributed with source code. 
The commercial database can be obtained [here](https://www.ip2location.com/database/ip2location). Edit this code line to replace the free database with the commercial version:

```python
database = ipl.IP2Location('geodata/IP2LOCATION-LITE-DB1.BIN','SHARED_MEMORY')
```

## Time of data processing

The processing may take a long time depending on the hardware. Precomputed results are provided to run the notebook quickly. Preprocessed is the historical dataset and geolocations. By default, the precomputed historical dataset is used. Set the values to False to process the raw data from scratch.

```python
precompdata = True
precomploc = True
```

# Links to used data
- RIPE Atlas archive (free) is available [here](https://ftp.ripe.net/ripe/atlas/probes/archive/)
- Country IP geolocation database (free) is available [here](https://lite.ip2location.com/ip2location-lite)
- Country IP geolocation database (commercial) can be obtained [here](https://www.ip2location.com/database/ip2location)
- Country border maps (free) are available [here](https://www.naturalearthdata.com/downloads/)

# Acknowledgment
This site or product includes IP2Location LITE data available from http://www.ip2location.com.
