# IMS Core – Testing and Validation

This directory documents the tests performed to validate the IMS core deployment.

## SIP Communication Test

A communication test was performed between two IMS subscribers:

- **Alice:** Calling subscriber
- **Bob:** Receiving subscriber

The SIP signaling exchange showed the following responses:

- `100 Trying`
- `180 Ringing`
- `200 OK`

These responses demonstrate that the SIP session signaling progressed successfully between the two subscribers.

## RTP Media Verification

RTPengine was running and detected by Kamailio during the tests.

However, successful end-to-end RTP audio transmission between Alice and Bob has not yet been confirmed.

Further media-plane testing is required.

## Test Environment

- Ubuntu 24.04
- Kamailio 6.1.5
- PyHSS
- RTPengine
