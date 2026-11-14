# W2-PM5: Network Scanning with Zenmap

**Target:** my own local network
**Environment:** Windows, Zenmap (Nmap GUI)

## Objective

Find the live hosts on my local subnet and record their IP and MAC addresses.

## Steps

1. Downloaded Zenmap from nmap.org and installed it.
2. Ran `ipconfig` in CMD. Local IP: [your IP]. Subnet: [your subnet].
3. Entered the subnet in Zenmap and ran the **Ping Scan** profile.
4. Recorded the live hosts and their addresses.
5. Opened the **Topology** tab, turned on the legend and saved the graphic as PDF (`topology.pdf`).

## Results

Live hosts found: [number] (including my PC)

| # | IP address | MAC address |
|---|------------|-------------|
| 1 | [192.168.56.1] | [] |

> For a public repo, hide or blur these addresses in the screenshots and topology PDF.

## Why it matters

A network map shows an attacker which devices to probe next. For defenders it shows what is connected, so unknown devices stand out.

## How to reduce the exposure

Scan your own network regularly, investigate unknown devices, and keep an up-to-date network diagram.

## Evidence

Screenshots are in `screenshots/` and the topology PDF is in this folder.
