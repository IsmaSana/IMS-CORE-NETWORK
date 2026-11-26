# P-CSCF Configuration

The Proxy Call Session Control Function (P-CSCF) is the first point of contact between an IMS user equipment and the IMS core network.

In this deployment, the P-CSCF handles SIP signaling, supports user registration procedures, and communicates with the other IMS components.

**SIP listening port:** 5060 (UDP/TCP)

**Diameter connection:** PyHSS on port 3868, through the configured Diameter interface.

The configuration files and implementation details will be documented here.
