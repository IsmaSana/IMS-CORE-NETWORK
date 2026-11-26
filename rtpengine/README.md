# RTPengine – Media Relay

RTPengine is deployed as the media relay component of this IMS environment.

It works alongside Kamailio to manage RTP media streams during SIP sessions. It can assist with media address rewriting and relay functions.

### Deployment Details

- **Component:** RTPengine
- **Control interface:** 127.0.0.1:2223 (UDP)
- **RTP port range:** 30000–40000
- **Configuration file:** `/etc/rtpengine.conf`
- **Installation environment:** Ubuntu 24.04

Kamailio communicates with RTPengine through its NG control interface.

The service was started and its availability was verified. End-to-end RTP audio transmission between Alice and Bob has not yet been confirmed.
