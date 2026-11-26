# DNS Configuration – Bind9

Bind9 is used as the DNS server for the IMS core network.

It provides name resolution for the IMS domain and the network components involved in SIP and Diameter communication.

### Deployment Details

- **Component:** Bind9
- **Role:** DNS resolution
- **DNS port:** 53
- **Installation environment:** Ubuntu 24.04

The DNS configuration supports the resolution of IMS-related hostnames used by Kamailio and PyHSS.

The zone configuration and DNS records will be documented here.
