# PyHSS – Home Subscriber Server

PyHSS is used as the Home Subscriber Server (HSS) in this IMS deployment.

It stores subscriber-related information and provides the subscriber data required by the IMS core during authentication and registration procedures.

### Deployment Details

- **Component:** PyHSS
- **Role:** Home Subscriber Server (HSS)
- **Diameter port:** 3868
- **API port:** 8080
- **Installation environment:** Ubuntu 24.04

PyHSS communicates with the Kamailio CSCF instances through the Diameter protocol.

Configuration details and relevant implementation steps will be documented in this directory.
