# Memprocfs Hunter
This script is a memory forensic wrapper to https://github.com/ufrisk/MemProcFS for memory speed analysis.
It's includes several hunting modules and ELK import with pre built hunting dashboards. It's have cool features like metadata and imports detection. Eventlog parsning. Yara and ClamAV to detect malicious files and memory injection detection. Happy Hunting ;)

The screenshots are generated using the memory dump from the Disobey 2020 Memory Forensics Workshop.

![image](https://user-images.githubusercontent.com/81682232/117827752-8d80a900-b271-11eb-9957-62f5876cd1b6.png)

![image](https://user-images.githubusercontent.com/81682232/117826229-4ba33300-b270-11eb-945d-32575549295a.png)

![image](https://user-images.githubusercontent.com/81682232/117827628-717d0780-b271-11eb-8e40-8c9706c0e297.png)

![image](https://user-images.githubusercontent.com/81682232/117828082-d0428100-b271-11eb-85bb-7f9717773e45.png)

![image](https://user-images.githubusercontent.com/81682232/117828243-f1a36d00-b271-11eb-8935-1f7f5edd67e2.png)

![image](https://user-images.githubusercontent.com/81682232/117828520-2c0d0a00-b272-11eb-9ba9-4282530e44fc.png)

![image](https://user-images.githubusercontent.com/81682232/117828626-4646e800-b272-11eb-857f-94532b1ba8b7.png)

# Important

If you run the eventlog parser module, the file is sometime locked by powershell for ca 60sec before release. Just wait...
- Thanks to https://cqureacademy.com/ for there awesome tool <b>CQEVTXRecovery.exe</b> for fixing corrupted evtx files.

![image](https://user-images.githubusercontent.com/81682232/117829014-a2aa0780-b272-11eb-8a6b-ed752d3544e2.png)

If you want to import the hunting dashboards to ELK you need to download and start the services on the local machine:

- https://www.elastic.co/downloads/elasticsearch
- https://www.elastic.co/downloads/kibana

Unzip and start the services:
- C:\elasticsearch-7.12.0-windows-x86_64\elasticsearch-7.12.0\bin\elasticsearch.bat
- C:\kibana-7.12.0-windows-x86_64\bin\kibana.bat

Run the <b>MemProcFS_ELKImport</b> to import the hunting dashboards

![image](https://user-images.githubusercontent.com/81682232/117829893-73e06100-b273-11eb-8bc7-ffb594e5ef32.png)

![image](https://user-images.githubusercontent.com/81682232/117874356-27137f00-b2a1-11eb-9d7f-e3d9d570b99c.png)

![image](https://user-images.githubusercontent.com/81682232/117831277-b35b7d00-b274-11eb-846d-baeb84f2cbf0.png)

# Installation
Easy as one, two ,three ;)

Download the lates release of MemProcFS
- https://github.com/ufrisk/MemProcFS/releases

Download the lates release of Dokan and run the installer
- https://github.com/dokan-dev/dokany/releases

Mount the image with MemProcFS

![image](https://user-images.githubusercontent.com/81682232/117924948-d890cf80-b2f6-11eb-8bb7-a2a80339b97f.png)

Download the lates release of MemProcFSHunter and start the script
- https://github.com/memprocfshunt/Memprocfshunter/releases

![image](https://user-images.githubusercontent.com/81682232/117924333-dbd78b80-b2f5-11eb-9efd-10d2c4c0d438.png)

![image](https://user-images.githubusercontent.com/81682232/117924612-47b9f400-b2f6-11eb-821f-8e2490baa0cb.png)

![image](https://user-images.githubusercontent.com/81682232/117924649-57d1d380-b2f6-11eb-9587-8cbf44c3da6b.png)

It's all done!! Have Fun!!
