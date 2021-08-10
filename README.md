# PRECIP Radar Scan (TW)

This project aims to help the radar operators to decide the RHI scan strategy (the azimuths for RHI sectors) in field campaign.\
The notebook in this project pulls the CWB latest radar image from https://www.cwb.gov.tw/V8/C/W/OBS_Radar.html, and plot azimuths from the specified radar location. For now, 

Convert Level-0 Storm Tracker (ST) data to Level-1 SHARPpy format for skew-T plot using SHARPpy.
The output ascii file can be directly read by SHARPpy for skew-T diagram.

More information on **SHARPpy**, please see: https://sharppy.github.io/SHARPpy/index.html

Last update - 20210526 - Hungjui Yu

## Dependencies

This script uses **pandas** for data management, and **metpy** for calculating meteorological variables.
More information on **metpy**, please see: https://unidata.github.io/MetPy/latest/index.html

## How to run?

```
python3 ST_L0_L1_SHARPpy.py [/path/to/ST/file/no_XXXX.csv] [log_launch_time_YYYYMMDDHHmmss]
```

The scripit us supported by python3.
