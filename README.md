# 5G-network-module-component-properties-analysis
Data analysis in python to study the effect of different components and properties of a 5G network module to improve signal transmission quality and efficiency.

**ABOUT THE DATA**:
In this work, I used a 5G trace dataset collected from a major Irish mobile operator. The dataset is generated from two mobility patterns (static and car), and across two application patterns(video streaming and file download). The dataset is composed of client-side cellular key performance indicators (KPIs) comprised of channel-related metrics, context-related metrics, cell-related metrics and throughput information. These metrics are generated from a well-known non-rooted Android network monitoring application, G-NetTrack Pro. To the best of my knowledge, this is the first publicly available dataset that contains throughput, channel and context information for 5G networks.

**DATASET COLUMNS:**
**Network mode**: This influences the data speeds your device can achieve. 5G is 20 Gbps peak data rates and 100+ Mbps average data rates more than 4G.

**Speed**: Speed at the time of measurement in km/h.

**Distance**: distance from serving cell.

**DataConnection_Type**: Mobile or WiFi.

**RSRP**: Reference Signal Received Power is a measurement of the received power level in a cell network. It represents an average power over cell-specific reference symbols carried inside distinct RE. RSRP is used for measuring cell signal strength/ coverage and therefore cell selection (dBm). The average power is a measurement of the power received from a single reference signal. -44dbm (good) to -140dbm (bad). The best value of RSRP is about -3dB and worst value can be -19.5dB. (To improve RSRP in LTE, use a signal booster. Cell phone boosters amplify your signal, increasing the signal strength RSRP).

**RSRQ**: Reference Signal Received Quality indicates the quality of the received signal and its range is typically -19.5dB (bad) to -3dB (good). This represents a ratio between RSRP and RSSI. Signal strength (signal quality) is measured across all resource elements (RE), including interference from all sources (dB). (Reasons for poor RSRQ include Bad RSRP; Overshooting from neighbor cells; Less inter-sector separation of the same site; High utilization)

**SNR**: Signal to Noise Ratio is the signal power to noise ratio in dB. A signal with an SNR value of 20dB or more is recommended for data networks, whereas an SNR value of 25dB or more is recommended for networks that use voice applications.

**CQI**: Channel Quality Indicator is used by the mobile to indicate the channel quality to the eNB (Base station). The CQI reported value is between 0 and 15. This indicates the level of modulation and coding the user equipment (UE) could operate. In HSDPA, the CQI value ranges from 0 to 30. 30 indicates the best channel quality and 0.1 indicates the poorest channel quality.

**RSSI**: Received Signal Strength Indicator is a measure of cellular signal strength. This represents a received power (wide-band) including a serving cell and interference and noise from other sources. From 0 (good) to -100 (bad). RSSI value of 55 is good. (Factors impacting RSSI include physical environment: physical obstacles to the radio wave propagation; physical environment: distance between transmitter and receiver; radio environment: interferences from other AP/clients on the network or neighbouring network).

**DL_bitrate**: current downlink bit rate at the time of measurement.

**UL_bitrate**: current uplink bit rate at the time of measurement.

**State**: I (idle), V (voice), D (data).

**PINGAVE**: average ping result from data sequence.

**PINGMIN**: minimum ping result from data sequence.

**PINGMAX**: maximum ping result from data sequence.

**PINGSTDEV**: standard deviation for ping statistic from data sequence.

**PINGLOSS**: ping loss in percents.

**CELLHEX**: Cell in hex format.

**NODEHEX**: Node in hex format.

**LACHEX**: Location Area Code in hex format.

**RAWCELLID**: cell id in raw form.

**NRxRSRP**: RSRP values for the neighbouring cells.

**NRxRSRQ**: RSRQ values for the neighbouring cells.

**RSRQ = N*RSRP/RSSI**, where N = number of used resource blocks.
