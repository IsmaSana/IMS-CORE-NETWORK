# S-CSCF – Serving Call Session Control Function

## Overview

The Serving Call Session Control Function (S-CSCF) is the central session-control element of the IMS architecture. It handles SIP registration, subscriber authentication, session management and routing of SIP requests.

In this implementation, the S-CSCF is deployed using Kamailio 6.1.5 and communicates with the PyHSS through the Diameter Cx interface.

## Network Configuration

| Service | Protocol | Port |
|---|---|---:|
| SIP signaling | UDP | 6060 |
| SIP signaling | TCP | 6060 |
| Diameter Cx | TCP | 3870 |

**IMS Domain:** `ims.mnc001.mcc001.3gppnetwork.org`

**S-CSCF FQDN:** `scscf.ims.mnc001.mcc001.3gppnetwork.org`

## Main Configuration Files

- `kamailio.cfg` – Main Kamailio configuration, including SIP routing and session-control logic.
- `scscf.cfg` – S-CSCF-specific parameters, network settings and database connection.
- `scscf.xml` – Diameter configuration used to communicate with the HSS.
- `dispatcher.list` – Configuration for external SIP destinations.

## Integration with Other IMS Components

The S-CSCF communicates with:

- **I-CSCF:** Receives SIP requests and participates in selecting the serving S-CSCF.
- **PyHSS:** Exchanges subscriber-related information through the Diameter Cx interface.
- **P-CSCF:** Participates in SIP session signaling through the IMS architecture.

## Deployment Notes

The configuration files are provided as deployment references. Before using them on another server, adapt IP addresses, database credentials and network parameters to the target environment.

The example IP address `192.0.2.10` is a documentation placeholder and must be replaced with the appropriate server address.

