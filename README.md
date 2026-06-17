# Wireshark Network Traffic Analysis and SOC Investigation

## Project Overview

This project demonstrates hands-on network traffic monitoring and analysis using Wireshark in a Linux-based SOC lab environment. Network packets were captured and analyzed to understand communication patterns, protocol behavior, and host interactions. A SOC-style investigation was conducted to identify visited domains, associated IP addresses, protocols used, and whether communications were encrypted.

## Objectives

* Capture live network traffic using Wireshark.
* Analyze common network protocols.
* Monitor host communications and endpoint activity.
* Investigate DNS resolutions and website access.
* Identify encrypted and unencrypted traffic.
* Perform basic SOC investigation procedures.

## Tools Used

* Ubuntu Linux
* Wireshark 4.6.4
* VirtualBox
* Firefox Browser
* Terminal Utilities (ping, ip, groups)

## Lab Environment

| Component         | Details      |
| ----------------- | ------------ |
| Operating System  | Ubuntu Linux |
| Capture Tool      | Wireshark    |
| Network Interface | enp0s3       |
| Browser           | Firefox      |
| Virtualization    | VirtualBox   |

## Protocols Analyzed

### ICMP

Used to verify network connectivity through Echo Request and Echo Reply packets.

### DNS

Captured DNS queries and responses to identify domain name resolutions.

### HTTP

Analyzed unencrypted web traffic using HTTP protocol.

### TLS/HTTPS

Examined encrypted communications over HTTPS using TLS 1.2 and TLS 1.3.

### TCP

Investigated reliable transport layer communications and session establishment.

## Traffic Statistics

### Traffic Distribution

* IPv4 Traffic: 96.2%
* IPv6 Traffic: 3.8%
* TCP Traffic: 96.2%
* TLS Traffic: 33.9%
* HTTP Traffic: 0.5%

### Most Active Hosts

* 10.0.2.15 (SOC Lab Host)
* 34.49.51.44
* 151.101.157.91

## SOC Investigation Findings

### Domains Observed

* github.com
* google.com
* wikipedia.org
* neverssl.com

### IP Addresses Observed

* 34.49.51.44
* 151.101.157.91
* Additional IPs resolved through DNS queries

### Protocols Used

* DNS
* ICMP
* HTTP
* TCP
* TLS

### Encryption Status

Encrypted communications were observed using:

* TLS 1.2
* TLS 1.3

Traffic on port 443 confirmed secure HTTPS sessions.

## Skills Demonstrated

* Packet Capture
* Network Traffic Analysis
* Protocol Analysis
* DNS Investigation
* SOC Investigation
* Endpoint Monitoring
* Traffic Statistics Analysis
* Wireshark
* Linux Networking
* Cybersecurity Monitoring

## Project Structure

Wireshark-Network-Traffic-Analysis/

├── Screenshots/

├── PCAP/

├── Report/

└── README.md

## Conclusion

This project successfully demonstrated network traffic capture and analysis using Wireshark. Various protocols including ICMP, DNS, HTTP, TLS, and TCP were analyzed to understand network behavior and communication patterns. The investigation confirmed both encrypted and unencrypted traffic, providing practical experience in network monitoring and SOC analysis workflows.
