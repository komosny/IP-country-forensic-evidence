# Country location evidence from IP address

Raw data and source code for the paper Evidential value of country location evidence obtained from IP address geolocation.

# Content

## Directories

- atlas - daily operational reports for Atlas devices 2015 to 2022 (raw data)
- figures - generated plots for commercial geolocation database IP2Location DB1
- geodata - free geolocation database IP2Location DB1 LITE
- geography - country border maps
- history - compiled historical dataset
- maps - Atlas coverage maps for countries
- precomp - precomputed historical data and IP locations

## Files
- notebook.inbp - notebook with source code
- enviroment.txt - python and module versions

# Reproducibility
The notebook with preloaded data reproduces the results for the free geolocation database.

## Database license

The notebook works by default with the free version of the geolocation database. The commercial version cannot be distributed with source code. 
To use the commercial database in the notebook, obtain it [here](https://www.ip2location.com/database/ip2location) and edit this code line to replace the free database with the commercial version:

```python
database = ipl.IP2Location('geodata/IP2LOCATION-LITE-DB1.BIN','SHARED_MEMORY')
```

## Time of data processing

Due to large data, the processing may take a long time depending on the hardware. Precomputed results are provided to run the notebook quickly. Preprocessed is the historical dataset and IP locations. By default, the precomputed results for the historical dataset are used. Set the values to False to process the raw data from scratch.

```python
precompdata = True
precomploc = True
```

# Links to used data
- RIPE Atlas archive (free) is available [here](https://ftp.ripe.net/ripe/atlas/probes/archive/)
- Country IP geolocation database (free) is available [here](https://lite.ip2location.com/ip2location-lite)
- Country IP geolocation database (paid) can be obtained [here](https://www.ip2location.com/database/ip2location)
- Country border maps (free) are available [here](https://www.naturalearthdata.com/downloads/)

# Acknowledgment
This site or product includes IP2Location LITE data available from http://www.ip2location.com.
