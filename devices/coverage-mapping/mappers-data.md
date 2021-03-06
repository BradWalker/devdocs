# Mappers Data

## Data

All data collected for this effort is publicly available. A full database CSV dump is updated daily for download below. Each hotspot that heard an uplink is referenced by _uplink\_id_ in the hotspots table. 

[uplinks.csv](https://coverage-dumps.s3-us-west-2.amazonaws.com/daily-csv-dumps/uplinks.csv)

Database Fields:

```text
id: unique identifier of uplinks
device_uuid: console device uuid
device_name: console device name
dev_eui: device eui
devaddr: device addr
timestamp: time uplink was received
payload: raw payload
fcnt: uplink count
port: uplink port
latitude: device latitude
longitude: device longitude
altitude: device altitude
hdop: GPS accuracy
sat: number of visible satellites
```

[hotspots.csv](https://coverage-dumps.s3-us-west-2.amazonaws.com/daily-csv-dumps/hotspots.csv)

Database Fields:

```text
id: unique identifier of hotspot reception
uplink_id: unique identifier of uplink
hotspot_name: hotspot name
hotspot_id: hotspot public address
latitude: hotspot latitude
longitude: hotspot longitude
rssi: uplink rssi
snr: uplink snr
spreading: uplink spreading
timestamp: time uplink was received
channel: uplink channel
status: uplink status
```

