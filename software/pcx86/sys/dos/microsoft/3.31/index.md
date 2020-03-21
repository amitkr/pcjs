---
layout: page
title: Microsoft MS-DOS 3.31
permalink: /software/pcx86/sys/dos/microsoft/3.31/
redirect_from: /disks/pcx86/dos/microsoft/3.31/
machines:
  - id: ibm5170-msdos331
    type: pcx86
    config: /configs/pcx86/xml/machine/5170/ega/640kb/rev1/machine.xml
    autoMount:
      A:
        name: MS-DOS 3.31 (1.44M Disk)
---

It's unclear where this [June 1989](#directory-of-ms-dos-331-144m-disk) release of MS-DOS 3.31 fits in the
MS-DOS timeline, because it comes *after* [MS-DOS 4.00](/disks/pcx86/dos/microsoft/4.00/) (October 1988) and
[MS-DOS 4.01](/disks/pcx86/dos/microsoft/4.01/) (April 1989).
Note that [COMPAQ MS-DOS 3.31](/disks/pcx86/dos/compaq/3.31/) existed as early as September 1987, raising the
question of whether there were *earlier* releases of Microsoft MS-DOS 3.31 as well.

Even though the majority of the files are dated June 1989, most of the copyright strings are unchanged from
[MS-DOS 3.30](/disks/pcx86/dos/microsoft/3.30/):

    Microsoft(R) MS-DOS(R)  Version 3.31                                            
                 (C)Copyright Microsoft Corp 1981-1987                              

Many of the utilities, such as `TREE.COM`, contain strings suggesting they are unchanged from MS-DOS 3.30:

    The MS-Dos Directory Path Display Utility
    (C)Copyright Microsoft Corp 1987
    Version 3.30

and indeed, with the exception of a one-byte difference in the utility's DOS version check, the 3.30 and 3.31
`TREE.COM` binaries *are* identical.

{% include machine.html id="ibm5170-msdos331" %}

### Directory of MS-DOS 3.31 (1.44M Disk)

	 Volume in drive A has no label

	Directory of A:\

	IO       SYS     23581 06-14-89  12:07p
	MSDOS    SYS     30672 06-11-89   4:33p
	COMMAND  COM     25276 06-01-89  12:00a
	4201     CPI     17089 06-01-89  12:00a
	5202     CPI       459 06-01-89  12:00a
	ANSI     SYS      1647 06-01-89  12:00a
	APPEND   EXE      5794 06-01-89  12:00a
	ASSIGN   COM      1530 06-01-89  12:00a
	ATTRIB   EXE     10656 06-01-89  12:00a
	BACKUP   COM     29976 06-19-89  12:29p
	CHKDSK   COM     11867 06-01-89  12:00a
	COMP     COM      4183 06-01-89  12:00a
	COUNTRY  SYS     11254 06-01-89  12:00a
	DATACOPY EXE     27313 05-25-89   2:34p
	DEBUG    COM     15944 06-01-89  12:00a
	DISKCOMP COM      5848 06-01-89  12:00a
	DISKCOPY COM      6264 06-01-89  12:00a
	DISPLAY  SYS     11259 06-01-89  12:00a
	DRIVER   SYS      1165 06-01-89  12:00a
	EDLIN    COM      7495 06-01-89  12:00a
	EGA      CPI     49065 06-01-89  12:00a
	EXE2BIN  EXE      3050 06-01-89  12:00a
	FASTOPEN EXE      3888 06-01-89  12:00a
	FC       EXE     15974 06-01-89  12:00a
	FDISK    COM     53275 06-01-89  12:00a
	FIND     EXE      6403 06-01-89  12:00a
	FORMAT   COM     19683 06-29-89  12:02p
	GRAFTABL COM      6216 06-01-89  12:00a
	GRAPHICS COM     13943 06-01-89  12:00a
	GWBASIC  EXE     80592 06-01-89  12:00a
	JOIN     EXE      9612 06-01-89  12:00a
	KEYB     COM      9041 06-01-89  12:00a
	KEYBOARD SYS     19735 06-01-89  12:00a
	LABEL    COM      2346 06-01-89  12:00a
	LINK     EXE     39172 06-01-89  12:00a
	MCONFIG  COM      1361 03-27-89  10:09a
	MODE     COM     15440 06-01-89  12:00a
	MORE     COM       282 06-01-89  12:00a
	NLSFUNC  EXE      3029 06-01-89  12:00a
	PRINT    COM      8995 06-01-89  12:00a
	PRINTER  SYS     13559 06-01-89  12:00a
	PROTO    SYS        54 12-06-88  10:50a
	RAMDRIVE SYS      8225 06-01-89  12:00a
	READPORT COM        39 10-27-88   8:34p
	REBOOT   COM        42 11-03-88   6:38a
	RECOVER  COM      5281 06-01-89  12:00a
	REPLACE  EXE     13234 06-01-89  12:00a
	RESTORE  COM     35650 06-01-89  12:00a
	SELECT   COM      4132 06-01-89  12:00a
	SETCMOS  COM        96 11-10-88   2:29a
	SETPORT  COM        24 12-09-88   7:02p
	SETSPD   COM       151 10-14-88   2:49p
	SETUP    COM        14 10-20-88   4:18p
	SHARE    EXE      8608 06-01-89  12:00a
	SORT     EXE      1946 06-19-89  12:30p
	SUBST    EXE     10552 06-01-89  12:00a
	SYS      COM      6127 06-01-89  12:00a
	TREE     COM      3540 06-01-89  12:00a
	UPDCFG   COM      7943 11-20-87   3:24p
	XCOPY    EXE     11216 06-01-89  12:00a
	       60 file(s)     740807 bytes

	Total files listed:
	       60 file(s)     740807 bytes
	                      700928 bytes free

NOTE: Like most of the directory listings PCjs provides, the above listing was produced by PC DOS 5.00.  However,
when MS-DOS 3.31 displays its own directory (see below), a time is not displayed for most of the files.

This is because those files have a 0x0000 timestamp, which technically is equivalent to midnight, but early versions
of DOS treated zero as an uninitialized timestamp.  On previous distribution disks, Microsoft used a timestamp of
0x0001 (two seconds past midnight) to indicate 12:00am, so this is just another indication that perhaps this was not
a fully baked retail release.

     Volume in drive A has no label
     Directory of  A:\
    
    COMMAND  COM    25276   6-01-89
    4201     CPI    17089   6-01-89
    5202     CPI      459   6-01-89
    ANSI     SYS     1647   6-01-89
    APPEND   EXE     5794   6-01-89
    ASSIGN   COM     1530   6-01-89
    ATTRIB   EXE    10656   6-01-89
    BACKUP   COM    29976   6-19-89  12:29p
    CHKDSK   COM    11867   6-01-89
    COMP     COM     4183   6-01-89
    COUNTRY  SYS    11254   6-01-89
    DATACOPY EXE    27313   5-25-89   2:34p
    DEBUG    COM    15944   6-01-89
    DISKCOMP COM     5848   6-01-89
    DISKCOPY COM     6264   6-01-89
    DISPLAY  SYS    11259   6-01-89
    DRIVER   SYS     1165   6-01-89
    EDLIN    COM     7495   6-01-89
    EGA      CPI    49065   6-01-89
    EXE2BIN  EXE     3050   6-01-89
    FASTOPEN EXE     3888   6-01-89
    FC       EXE    15974   6-01-89
    FDISK    COM    53275   6-01-89
    FIND     EXE     6403   6-01-89
    FORMAT   COM    19683   6-29-89  12:02p
    GRAFTABL COM     6216   6-01-89
    GRAPHICS COM    13943   6-01-89
    GWBASIC  EXE    80592   6-01-89
    JOIN     EXE     9612   6-01-89
    KEYB     COM     9041   6-01-89
    KEYBOARD SYS    19735   6-01-89
    LABEL    COM     2346   6-01-89
    LINK     EXE    39172   6-01-89
    MCONFIG  COM     1361   3-27-89  10:09a
    MODE     COM    15440   6-01-89
    MORE     COM      282   6-01-89
    NLSFUNC  EXE     3029   6-01-89
    PRINT    COM     8995   6-01-89
    PRINTER  SYS    13559   6-01-89
    PROTO    SYS       54  12-06-88  10:50a
    RAMDRIVE SYS     8225   6-01-89
    READPORT COM       39  10-27-88   8:34p
    REBOOT   COM       42  11-03-88   6:38a
    RECOVER  COM     5281   6-01-89
    REPLACE  EXE    13234   6-01-89
    RESTORE  COM    35650   6-01-89
    SELECT   COM     4132   6-01-89
    SETCMOS  COM       96  11-10-88   2:29a
    SETPORT  COM       24  12-09-88   7:02p
    SETSPD   COM      151  10-14-88   2:49p
    SETUP    COM       14  10-20-88   4:18p
    SHARE    EXE     8608   6-01-89
    SORT     EXE     1946   6-19-89  12:30p
    SUBST    EXE    10552   6-01-89
    SYS      COM     6127   6-01-89
    TREE     COM     3540   6-01-89
    UPDCFG   COM     7943  11-20-87   3:24p
    XCOPY    EXE    11216   6-01-89
           58 File(s)    700928 bytes free