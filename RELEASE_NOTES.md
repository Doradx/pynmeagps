# pynmeagps Release Notes

### RELEASE 1.0.4

ENHANCEMENTS:

1. The nmeadump.py example has been moved into the pynmeagpscli module and configured as a setup entry point. It is now available as a simple command line utility. See README for usage.

### RELEASE 1.0.3

FIXES:

1. Fixed diffAge field type in GGA payload definition.

### RELEASE 1.0.2

FIXES:

1. Fixed typo in VTG payload definition - `cogT` is now `cogt`. Test script updated.

### RELEASE 1.0.1

FIXES:

1. Fixed typo in GBS payload definition - `effLon` is now `errLon`. Test script updated.
2. Fixed cosmetic typo in nmeafile.py example - functionality not affected.

### RELEASE 1.0.0

CHANGES:

1. Marked to v1.0.0 Production/Stable. No other functional changes.

### RELEASE 0.1.8-beta

FIXES:

1. NMEA PUBX msgId parsed as str rather than int.

ENHANCEMENTS:

2. nmeatypes_core.py NMEA_MSGID table split into standard and proprietary dicts. 
3. nmeapollall.py example added.

### RELEASE 0.1.7-beta

ENHANCEMENTS:

1. Following standard message types added: AAM, APA, APB, BOD, BWC, MSK, MSS, RMA, RMB, STN, VBW, WPL, XTE, 
2. Following proprietary message types added: (Garmin) GRME, GRMM, GRMZ

Further types will be added in subsequent releases. Shout or submit PR if you want yours prioritised.

### RELEASE 0.1.6-beta

ENHANCEMENTS:

1. message types HDG, HDM, HDT, RTE added
2. msgdesc() helper method added to get description of NMEA message type.
3. construction of proprietary messages (talker = 'P') made more consistent with standard messages.

FIXES:

1. nominal value for HX (hex) attribute type updated to integer rather than string (only currently affects RLM message type).


### RELEASE 0.1.5-beta

CHANGES:

1. Optional arguments to NMEARreader constructor and parse() method have been changed to **kwargs rather than args for future flexibility. See docstrings for usage.

### RELEASE 0.1.4-beta

ENHANCEMENTS:

1. Add Garmin proprietary NMEA sentences GET and SET.

### RELEASE 0.1.3-beta

ENHANCEMENTS:

1. Parse validate flag added to NMEAReader.read() method, defaults to VLCKSUM (1 - check checksum only); other options are VALNONE = 0, 
VALMSGID = 2. Options can be ANDed. Examples updated accordingly.

### RELEASE 0.1.2-beta

1. Constructor enhanced to allow NMEAMessage to be created using typed values.

### RELEASE 0.1.1-beta

1. README.MD and GitHub workflow/coverage updated

### RELEASE 0.1.0-beta

1. Initial public beta release
