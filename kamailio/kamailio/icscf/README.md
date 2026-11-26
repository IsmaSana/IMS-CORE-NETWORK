# I-CSCF Configuration

The Interrogating Call Session Control Function (I-CSCF) is responsible for identifying the appropriate S-CSCF for an IMS subscriber.

In this deployment, the I-CSCF communicates with the HSS through the Diameter protocol to retrieve subscriber-related information and select the appropriate serving CSCF.

**SIP listening port:** 4060 (UDP/TCP)

**Diameter connection:** PyHSS HSS

The configuration files and implementation details will be documented here.
