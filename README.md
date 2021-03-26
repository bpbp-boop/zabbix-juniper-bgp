# Zabbix Juniper BGP template
A template to pull BGP peer data from SNMP for Zabbix. Should work with any Juniper device that supports `BGP4-V2-MIB-JUNIPER`

## Installing
Import the .yaml file under Configuration > Templates > Import.

## Item prototypes (per peer)
- Administrative status
- Established time
- IPv4 prefixes accepted
- IPv4 prefixes advertised
- IPv4 prefixes received
- IPv4 prefixes rejected
- IPv6 prefixes accepted
- IPv6 prefixes advertised
- IPv6 prefixes received
- IPv6 prefixes rejected
- Last received error
- Last sent error
- Peer state

## Trigger prototypes (per peer)
- Peer down
- Peer losing more than 20% of received prefixes

## Value maps
- BGP peer administrative status
- BGP peer state

## About
I wanted to monitor BGP peers using Zabbix without using any external scripts

Inspired by https://github.com/Prototype-X/Zabbix-Template-Juniper-MX-BGP4-ipv4-ipv6.