rmcat-adaptive-fec-code
=======================

The proposed mechanism uses Forward Error Correction (FEC) encoded RTP packets (redundant packets) along side the media packets to probe for available network capacity.  A straightforward interpretation is, the sending endpoint increases the transmission rate by keeping the media rate constant but increases the amount of FEC.  If no losses and discards occur, the endpoint can then increase the media rate. If losses occur, the redundant FEC packets help in recovering the lost packets. Consequently, the endpoint can vary the FEC bit rate to conservatively (by a small amount) or aggressively (by a large amount) probe for available network capacity.

### Repository structure 
```
+ -ns2 
+ -gstreamer
```

### Referring to the Code

If you have used the code in this repository for your research, please use the MMSys paper as the reference.

> Nagy M., Singh V., Ott J., Eggert L., Congestion Control using FEC for Conversational Multimedia Communication, Proc. of ACM Multimedia Systems, Singapore, SG, Mar, 2014, [ACM](http://dl.acm.org/citation.cfm?id=2557649)

The BibTeX code snippet is:
```
@inproceedings{Nagy14:FEC,
 author = {Nagy, Marcin and Singh, Varun and Ott, J\"{o}rg and Eggert, Lars},
 title = {Congestion Control Using FEC for Conversational Multimedia Communication},
 booktitle = {Proceedings of the 5th ACM Multimedia Systems Conference},
 series = {MMSys '14},
 year = {2014},
 isbn = {978-1-4503-2705-3},
 location = {Singapore, Singapore},
 pages = {191--202},
 numpages = {12},
 doi = {10.1145/2557642.2557649},
 acmid = {2557649},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {FEC, RMCAT, RTP, WebRTC, congestion control},
} 
```
