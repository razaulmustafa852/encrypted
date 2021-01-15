# Real-Time, Machine Learning Approach to Predict Video-QoE for Encrypted Streaming Traffic in 5G Networks

Tools required to stream DASH video content

  - Mininet
  - goDASHBED
  - Caddy Web-server
  - 5G real traces

You can also download the dataset to play with DASH content QoS and QoE features:
  - The dataset have QoS features collected from pcaps named qos_file.csv
  - QoE logs of each experiments named qoe_file.csv
 
## Installation

The topology to re-produce same results is named topo.py and stream.py. You can define your requirements in stream.py. Where you can define number of hosts streaming DASH content, ABS algorithm, Server Type (TCP, QUIC), Web-server type etc.
Each time the experiments will create a directory in working location that contains goDASH logs + pcaps. After that please run single_0.5.py to extract QoS features from pcap for every 0.5s slot.

```sh
$ sudo python3 stream.py
```

