# MODULE 4 * Enumeration

## CONCEPTS

### Techniques:

* Extract user names using email IDs
* Extract information using default passwords
* Brute force Active Directory
* Extract information using DNS Zone Transfer
* Extract user groups from Windows
* Extract user names using SNMP

### Services and Ports to Enumerate

* TCP/UDP 53: DNS Zone Transfer
* TCP/UDP 135: MS RPC Endpoint Mapper
* UDP 137: NetBIOS Name Service (NBNS)
* TCP 139: NetBIOS Session Service (SMB over NetBIOS)
* TCP/UDP 445: SMB over TCP (Direct Host)
* UDP 161: SNMP
* TCP/UDP 389: LDAP
* TCP/UDP 3268: MS Global Catalog
* TCP 25: SMTP
* TCP/UDP 162: SNMP Trap
* UDP 500: ISAKMP/Internet Key Exchange (IKE)
* TCP/UDP 5060,5061: Session Initiation Protocol (SIP)

## NETBIOS

NetBIOS name: Unique computer name 16char ASCII.

* 1-15 device name
* 16 service name or name record type

Ports:

* UDP 137: NetBIOS Name Service (NBNS)
* UDP 138: Datagram Services
* TCP 139: NetBIOS Session Service (SMB over NetBIOS)

Can obtain:

* List of computers that belong to a domain
* List of shares on the individual hosts
* Policies and passwords

## SNMP

SNMP Passwords:

* Read community string
* Read/write community string

## LDAP



## LDAP

## NTP

## SMTP and DNS

## Other

## COUNTERMEASURES

## PEN TESTING