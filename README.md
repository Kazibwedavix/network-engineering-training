# Lab 01 — Basic Office Network

## Objective
To set up a basic network including 3 pc's i router and a switch 
Ensure that the pc's can ping each other showing successful communication
## Topology
<img width="1366" height="720" alt="Screenshot 2026-04-22 001331" src="https://github.com/user-attachments/assets/29b77598-d93d-4866-9c21-8be37e5d0ef9" />


## Network Details
| Device | Interface | IP Address    | Subnet Mask   |
|--------|-----------|---------------|---------------|
| Router | gig0/0     | 192.168.10.1  | 255.255.255.0 |
| PC1    | NIC       | 192.168.10.10 | 255.255.255.0 |
| PC2    | NIC       | 192.168.10.11 | 255.255.255.0 |
| PC3    | NIC       | 192.168.10.12 | 255.255.255.0 |

## To the router i used the  following configuration 
\```
enable
configure terminal
interface fastethernet 0/0
ip address 192.168.10.1 255.255.255.0
no shutdown
\```

## What I Learned
- How to assign static IPs to devices
- How a switch forwards traffic using MAC address tables
- Why a default gateway is needed to leave a subnet

## Ater carefull implementation the was succcessful pings on all the cpmputers 
- PC1 → PC2: ✅ Success
- PC1 → PC3: ✅ Success
- PC2 → PC3: ✅ Success
