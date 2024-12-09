# jair-altair
Serial Virtual Drive CP/M 2.2b for JAIR SBC

# Booting
Put `ALTBOOT.HEX` on your SD card.

Connect JAIR Port 1 to the Serial Drive Server with the baud rate set to 57.6K.

Mount the 8MB disk image to Drive 0.

Boot the JAIR and load `ALTBOOT.HEX`.

```
ALTAIR/IMSAI 8080 CPU BOARD BOOT LOADER - Josh Bensadon v2.5 Sep 3, 2018
<D> -SD Card Directory
<R> -RAM Test
<V> -View Load
> .d
INIT_FAT 
Init SD Type#1 ACMD41+MBR S Type06 PBR S VOL=JAIR128M    SYS=FAT16   
DIRECTORY:
SPOTLI~1.       BIOS.HEX        _BIO~1.HEX      CPMDISKS.TXT    _CPMDI~1.TXT
DISK-A.BIN      _DISK-~1.BIN    DISK-B.BIN      _DISK-~2.BIN    DISK-C.BIN
_DISK-~3.BIN    DISK-D.BIN      _DISK-~4.BIN    ALTBOOT.HEX     TRASHE~1.

ENTER 8.3 FILE NAME> altboot.hex
ALTBOOT.HEX -EXISTS
FILE SIZE=0x000001F2

-EOF-
Execute at:FC00


64K CP/M 2.2b v1.0
For Altair 8Mb Virtual Serial Drive for JAIR

A0>ls
Name    Ext Bytes   Name    Ext Bytes   Name    Ext Bytes   Name    Ext Bytes
ASM     COM    8K | L80     COM   12K | NSWP    COM   12K | STAT    COM    8K
BIOS    ASM   64K | LADDER  COM   40K | PCGET   COM    4K | SUBMIT  COM    4K
BOOT    ASM    8K | LADDER  DAT    4K | PCPUT   COM    4K | SURVEY  COM    4K
DDT     COM    8K | LOAD    COM    4K | PIP     COM    8K | SYSGEN  COM    4K
DRIVES  TXT    4K | LS      COM    4K | R       COM    4K | W       COM    4K
DUMP    ASM    8K | M80     COM   20K | SERBOOT ASM    8K | WM      COM   12K
DUMP    COM    4K | MAC     COM   12K | SERBOOT HEX    4K | WM      HLP    4K
ED      COM    8K | MBASIC  COM   24K | STARINS BAS    8K | XSUB    COM    4K
FINDBAD COM    4K | MBASIC45COM   20K | STARTREKBAS    8K
IOBYTE  TXT    4K | MOVCPM8SCOM   12K | STARTRK BAS   20K
38 File(s), occupying 396K of 8168K total capacity
472 directory entries and 7772K bytes remain on A:
A0>
```
