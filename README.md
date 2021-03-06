# EWBF-0.3.4b
EWBF's CUDA Equihash Miner for NVIDIA GPU

Quick Start Guide

Download the miner using the link below.

Windows / Linux: <EWBF Miner>

Edit ZHash-Start.bat file with your favorite text editor.

1. Set the --server <URL> and --port <number>
2. Change the <yourWallet> with your wallet address.
3. Save and exit.

Example: miner.exe --server eu1.zhash.pro --port 6057 --user yourWallet.workerName --pass x --pec 

Run EWBF Miner by double clicking start.bat

Approximate hash rates:

GTX 1080: 500 Sols/s
GTX 1070: 435 Sols/s
GTX 1060: 295 Sols/s


#Help

--help, -h          Show short help.

--server            Stratum server only hostname or ip address.

--port              Stratum server port.

--user              Stratum user.

--pass              Stratum password.

--cuda_devices      Space-separated list of cuda devices. Without this option all devices are used.

--solver            Disable benchmark and use specified solver. Allowed values from 0 to 3.
                    Started from version 0.3.0b this option allow you to set the solver for each card separately at this manner: --solver 0 0 0 0
                    For example if you have 4 cuda devices and you do not use option --cuda_devices 
                    then --solver 0 1 2 3 will be applied to devices 0 1 2 3 accordingly.
                    if you set --solver 0 then this value will be applied to all devices
                    if you set --cuda_devices 3 2 1 then solver values will be applied in this order.

--eexit             Exit in case of error. Value 1 exit if miner cannot restart workers.
                    Value 2 if lost connection with the pool. 3 both cases.

--log               Create file miner.log in directory of miner.
                    Allowed values 1 and 2. 1 only errors, 2 will repeat console output.

--logfile           Set custom filename.

--config            Specifies the configuration file, when the configuration file is used, all other command-line parameters are ignored.

--intensity         Specifies maximum intensity, allowed values 1 - 64. Lower value, lower speed and gpu usage.

--tempunits         Temperature units, allowed values: C for celsius, F for fahrenheit and K for kelvin :)).

--templimit         Temperature limit, gpu will be stopped if this limit is reached.
                    And when temperature go below this limit gpu will be runned again.
                    Note: If this limit is too low and miner stops this gpu too frequently 
                    and option --eexit equal 1 or 3 then after three unsuccessfull starting attempts miner will exit.

--api               Enable api without an argument will be listen on 127.0.0.1:42000,
                    You can set listen address as an argument for example: --api 0.0.0.0:12345
                    Allowed ports 1000 - 65535.
