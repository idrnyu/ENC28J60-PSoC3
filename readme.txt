ENC28J60 with the PSoC3
----------------------

This project is basically an open source TCP/IP network stack,based around the ENC28J60 and a PSoC3 chip controlling it.

Current status: 
-ENC28J60 Hardware Test Code Done.(ENC28J60-HWTest.cydsn)
-ARP Request/Reply Code Done.(ENC28J60-ARPTest.cydsn)
-WebServer done.  |
-DNS Done.        |--(ENC28J60-BasicWebserver.cydsn)
-Webclient done.  |
-COSM Example(Upload Data) Added.(ENC28J60-COSMExample.cydsn)
-COSM Read Feed Example(Download data) Added.(ENC28J60-COSMReadExample.cydsn)
-Generic UDP RX/TX Example Added.(ENC28J60-BasicUDP.cydsn)

--Update 8 July 2012 - WebClient works fine now.Thanks to duncanspumpkin(http://mostlyprog.wordpress.com) who pointed out that I hadnt zero-ed out the checksum(before calculation) in the SYN sending function.

Todo:
1.Watchdog Routine.
2.NTP(?)
3.WOL(?)

This code has been tested with:
  Hardware: CY8CKIT-030 with ENC28J60 module from http://www.embeddedmarket.com/products/ENC28J60-Ethernet-Module/
  Software: PSoC Creator 2.1 with cy_boot 3.0
            PyUDPComm v1.0(https://github.com/kmmankad/PyUDPComm) for the UDP example.

Based heavily on the work by Duncan Frost for the MSP430.
Credits and sincere thanks to him.


-kmmankad

http://kmmankad.blogspot.com

This work is licensed under a Creative Commons Attribution-ShareAlike 3.0 Unported License.

Last Updated on 10-July-2012.