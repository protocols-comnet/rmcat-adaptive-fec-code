rmcat-adaptive-fec-code
=======================

The proposed mechanism uses Forward Error Correction (FEC) encoded RTP packets (redundant packets) along side the media packets to probe for available network capacity.  A straightforward interpretation is, the sending endpoint increases the transmission rate by keeping the media rate constant but increases the amount of FEC.  If no losses and discards occur, the endpoint can then increase the media rate. If losses occur, the redundant FEC packets help in recovering the lost packets. Consequently, the endpoint can vary the FEC bit rate to conservatively (by a small amount) or aggressively (by a large amount) probe for available network capacity.
