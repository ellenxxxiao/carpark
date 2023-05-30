# CITS4419 Group Project 2023
## Real-time Parking Alert System with VANET
<br>
The data is collected with TTGO transmitters and receivers, using LoRa parameters:


| Bandwidth | Speading Factor | Coding rate | Power | Frequency |
| --------- | ----------------| ----------- | ----- | --------- |
|   250E3   |        12       |      5      |   20  |   9233E5  |

<br>

### Data

We have collected data for 8 car parks (P1, P3, P8, P18, P26, P31, P33, P43) in UWA Crawley campus. 

The data are stored in 8 csv files. The location coordinates for the car parks are store in `carpark_locs.txt`.

<br>

The columns:
- `R_Time` - Receive time
- `Comm_ID` - Prefix for all transmitted messages, for disambiguation
- `Pkt_Set` - Index of set
- `Pkt_ID` - Index of packet within set
- `S_Lat` - Transmitter Latitude
- `S_Lng` - Transmitter Logitude
- `Pkt_BW` - Bandwidth (250E3)
- `Pkt_CR` - Coding Rate (5)
- `Pkt_Freq` - Frequency (9233E5)
- `Pkt_SF` - Spreading Factor (12)
- `Pkt_Tx_Pwr` - Transmission Power (20)
- `Pkt_RSSI` - Packet RSSI
- `Now_RSSI` - Current RSSI of the ratio
- `Pkt_SNR` - Packet SNR
- `R_Lat` - Receiver Latitude
- `R_Lng` - Receiver Longitude

<br>

### Code
Version of packages used in processing code `carpark.ipynb`:
| package | version |
| ------- | ------- |
| pandas | 1.5.3 |
| plotly | 5.9.0 |
| geopy | 2.3.0 |
| geopandas | 0.12.2 |