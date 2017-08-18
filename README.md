OVERVIEW
========
ODR-DabMod is a *DAB (Digital Audio Broadcasting)* modulator compliant
to ETSI EN 300 401. It is the continuation of the work started by which was
developed by the Communications Research Center Canada on CRC-DabMod, and
is now pursued in the
[Opendigitalradio project](http://opendigitalradio.org).


ODR-DabMod is part of the ODR-mmbTools tool set. More information about the
ODR-mmbTools is available in the *guide*, available on the
[Opendigitalradio mmbTools page](http://www.opendigitalradio.org/mmbtools).

Short list of features:

- Reads ETI and EDI, outputs compliant COFDM I/Q
- Supports native DAB sample rate and can also
  resample to other rates
- supports all four DAB transmission modes
- Configuration file support, see doc/example.ini
- Integrated UHD output for [USRP devices](https://www.ettus.com/product)
  - Tested for B200, B100, USRP2, USRP1
  - With WBX daughterboard (where appropriate)
- Experimental [SoapySDR](https://github.com/pothosware/SoapySDR/wiki) output
  - Can be used to drive the [LimeSDR board](https://myriadrf.org/projects/limesdr/), the [HackRF](https://greatscottgadgets.com/hackrf/) and others.
- Timestamping support required for SFN
- GPSDO monitoring (both Ettus and [ODR LEA-M8F board](http://www.opendigitalradio.org/lea-m8f-gpsdo))
- A FIR filter for improved spectrum mask
- Logging: log to file, to syslog
- ETI sources: ETI-over-TCP, file (Raw, Framed and Streamed) and ZeroMQ
- A Telnet and ZeroMQ remote-control that can be used to change
  some parameters during runtime
- ZeroMQ PUB and REP output.
- Ongoing work about digital predistortion for PA linearisation.
  See dpd/README.md

The src/ directory contains the source code of ODR-DabMod.

The doc/ directory contains the ODR-DabMod documentation, and an example
configuration file.

The lib/ directory contains source code of libraries needed to build
ODR-DabMod.

INSTALL
=======
See the INSTALL file for installation instructions.

LICENCE
=======
See the files LICENCE and COPYING

CONTACT
=======
Matthias P. Braendli *matthias [at] mpb [dot] li*

Pascal Charest *pascal [dot] charest [at] crc [dot] ca*

With thanks to other contributors listed in AUTHORS

http://opendigitalradio.org/
