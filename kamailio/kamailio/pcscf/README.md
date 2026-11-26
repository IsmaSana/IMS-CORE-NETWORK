# P-CSCF Configuration

The Proxy Call Session Control Function (P-CSCF) is the first point of contact between an IMS user equipment and the IMS core network.

In this deployment, the P-CSCF handles SIP signaling, supports user registration procedures, and communicates with the other IMS components.

**SIP listening port:** 5060 (UDP/TCP)

**Diameter connection:** PyHSS on port 3868, through the configured Diameter interface.

The configuration files and implementation details will be documented here.


### Configuration adapted for this deployment

This configuration was adapted to integrate the P-CSCF into my IMS laboratory environment.

The following parameters may need to be changed before testing on another machine:

- **IP addresses:** Replace the example IP address with the IP address of your IMS server.
- **Database credentials:** Replace `CHANGE_ME` with the password configured in MariaDB.
- **Database connection:** Ensure that the database name, username and connection address match your local installation.
- **Network interfaces:** Adapt the interface settings to your network environment.

The original working configuration was tested in my Ubuntu 24.04 IMS environment. These files are provided as reference configurations and must be adapted before deployment.
