# EWBF-0.3.4b (Zcash, Horizen)
EWBF's CUDA Equihash Miner for NVIDIA GPU

## Quick Start Guide

Download the miner using the link below.

**NOTE**: Chrome browser may block the download. Use Mozilla Firefox or another browser.

[Download EWBF 0.3.4b Windows Version](https://github.com/zhashpro/EWBF-0.3.4b/raw/main/EWBF-0.3.4b.rar)

Extract the archive and edit _ZHash-Start.bat_ file with your favorite text editor.

1. Set the --server _URL_ and --port _number_
2. Change _yourWallet_ to your wallet address
3. Save and exit

**Example for Zcash**: miner.exe --server _eu1.zhash.pro_ --port _6058_ --user _yourWallet_.workerName --pass x --pec

**Example for Horizen**: miner.exe --server _eu1.zhash.pro_ --port _3058_ --user _yourWallet_.workerName --pass x --pec

Run EWBF Miner by double clicking _ZHash-Start.bat_

Approximate hash rates:

GTX 1080: 500 Sols/s

GTX 1070: 435 Sols/s

GTX 1060: 295 Sols/s

See Help.txt for more details and command line switches.
