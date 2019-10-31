# MODULE 3 * Scanning Netwokrs

## CONCEPTS

### Types

* Port scanning
* Network scanning
* Vulnerability scanning

### Objectives

Discover:

* Live hosts, IP, open ports
* OS, Arquitecture
* Services
* Services: Applications or versions
* Vulnerabilities

### TCP flags

* SYN
* ACK
* PSH - Push
* URG
* FIN
* RST

### TCP/IP Comunication

![TCP/IP Communication diagram](TCPIP_Communication.gif)

## SCANNING TOOLS

[Tools](Tools.md)

## SCANNING TECHNIQUES

[Principal ports list](common-ports.pdf)

### ICMP

* ICMP Scanning
* Ping Sweep
* ICMP Echo scanning

### TCP

* Open TCP
  * TCP Connect / Full Open Scan
* Stealth TCP
  * Half-open Scan
  * Inverse TCP Flag
    * Xmas Scan
    * FIN Scan
    * NULL Scan
  * ACK Flag Probe
    * TTL-based ACK flag
    * WINDOW based ACK flag
    * 
* Third Party and Spoofed TCP
  * IDLE/IP ID Header Scanning

### UDP

* UDP Scanning

### SSDP y List scaning

## SCANING BEYOND IDS AND FIREWALL

Evasion techniques:

### Packet fragmentation

### Source Routing

### IP Adress Decoy

### IP Adress Spoofing

 IP Spoofing Detection:

 * Direct TTL probes
 * IP Identification number (IPID)
 * TCP Flow Control

 Countermeasures:

 * Avoid trust relationships
 * Use fw and filtering mechanisms
 * Use random seq. numbers
 * Ingress filtering
 * Egress filtering
 * Use encryption
 * SYN flooding countermeasures

### Proxy Server

Proxy chaining.

[Tools](Tools.md)

### Anonymizers.

Reasons:

* Ensuring privacy
* Accessing govermment-restricted content
* Protection against online attacks
* Bypassing IDS and FW rules

Types:

* Networked Anon.
* Single-Point Anon.

## BANNER GRABBING

Types

* Active Banner Grabbing
* Pasive Banner Grabbing
  * Error logs
  * Sniffing network traffic
  * From page extensions

Areas that determine the OS:

* TTL of the packets.
* Window size.
* Whether the DF bit is set.
* TOS (Type of Service)

Countermeasures

* Disabling or Changing Banner
  * Display false banners.
  * Turn off unnecesary services.
  * Use ServerMask tools.
  * ServerMask removes HTTP header, provides false signatures and also provides the optio of eliminating file extensios such as .asp or .aspx
  * Apache: change banner information.
  * Change the ServerSignature to ServerSignatureOff in the httpd.conf file.
* Hiding File Extensions from Web Pages
  * Hide file extensios to mask the web technology
  * Change app. mappings such as .asp with .htm
  * Apache users can use mod_negotiation directives
  * IIS users use tools such as PageXchanger



## DRAW NETWORK DIAGRAMS

## SCANNING PEN TESTING

Help de sysadmin to:

* Close unused ports
* Disable unnecessary services
* Hide or customize banners
* Troubleshoot service configuration errors
* Calibrate FW rules to impose more restriction

Pen-test:

1. Perform host discovery
2. Perform port scanning
3. Scan beyond IDS and FW
4. Perform banner grabbing or OS fingerprinting
5. Draw network diagrams
6. Document all the findings




