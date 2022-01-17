# obfs4-mingan
Dataset for 'Towards Comprehensive Analysis of Tor Hidden Service Access Behavior Identification Under Obfs4 Scenario'.

We uploaded the experimental data to Baidu Netdisk. link：[BaiduNetdisk](https://pan.baidu.com/s/1kafKyemzmdEsyRnFlrV8NQ)

Extraction code：2rfw

The tree structure of the dataset is:

```
dataset_Obfs4-MingAn
├── log
│   ├── client0_server0
│   ├── client0_server1
│   ├── client0_server2
│   ├── client1_server0
│   ├── client1_server1
│   ├── client1_server2
│   ├── client2_server0
│   ├── client2_server1
│   └── client2_server2
└── tcp
    ├── client0_server0
    ├── client0_server1
    ├── client0_server2
    ├── client1_server0
    ├── client1_server1
    ├── client1_server2
    ├── client2_server0
    ├── client2_server1
    └── client2_server2
```

**clientdata** is the stream related to accessing website content, **clientrp** is the stream related to accessing hidden service content, and **createfast** is the stream related to downloading cached files.

For each trace, there is a txt file recording the TCP sequence in the tcp folder, and a corresponding Tor log file in the log folder with the same name. The first number of the filename is the type of target domain(0 for clientdata, 1 for clientrp).

For example, the following **TCP sequence file** and  **Tor log file** come from the same trace, and the target domain is clientdata.

```
TCP sequence file:
0-1.txt

Tor log file:
0-1.log
```
