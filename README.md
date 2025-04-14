# CBT290
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 290 is the documentation and source for GPSAM from the    *   FILE 290
//*           Yale Computer Center, written by Howard Gilbert.      *   FILE 290
//*           The documentation, which is in member $$$DOC, is in   *   FILE 290
//*           FBA format, LRECL=80.  The source for GPSAM is in     *   FILE 290
//*           the rest of this file.                                *   FILE 290
//*                                                                 *   FILE 290
//*           GPSAM lets you write your own "access method" and     *   FILE 290
//*           make it look like a sequential dataset to any         *   FILE 290
//*           application program or utility.  It can be used to    *   FILE 290
//*           provide DBMS, VTAM, TSO Fullscreen, BTAM, or          *   FILE 290
//*           specialized device support.                           *   FILE 290
//*                                                                 *   FILE 290
//*           SIMPLE:  Installs on any MVS system.  No IBM code     *   FILE 290
//*           is modified.  Takes only a few minutes to run         *   FILE 290
//*           linkedit steps and build procedures.                  *   FILE 290
//*                                                                 *   FILE 290
//*           SMALL:   700 bytes in LPA.  160 bytes in private      *   FILE 290
//*           address space.                                        *   FILE 290
//*                                                                 *   FILE 290
//*           SAFE:    Only one instruction executes in key 0 and   *   FILE 290
//*           modifies a general system control block.  Another     *   FILE 290
//*           18 instructions operate in a system key and only 4    *   FILE 290
//*           of them change storage, storing values in job         *   FILE 290
//*           related control blocks in the private area.  Even     *   FILE 290
//*           the most conservative installation can desk check     *   FILE 290
//*           the single authorized csect several times over in     *   FILE 290
//*           an hour.                                              *   FILE 290
//*                                                                 *   FILE 290
//*           UNIVERSAL:  While a system programmer must install    *   FILE 290
//*           the package in authorized libraries, any              *   FILE 290
//*           application programmer can write his own "access      *   FILE 290
//*           method" in assembler and use it from his own          *   FILE 290
//*           programs.  The user specifies the module name on      *   FILE 290
//*           his DD card or in the TSO allocation of the           *   FILE 290
//*           ddname.  These user modules run in problem state      *   FILE 290
//*           and can come from any library.  Control is given      *   FILE 290
//*           to the routine from the OPEN, CLOSE, GET, PUT,        *   FILE 290
//*           READ, or WRITE statements.                            *   FILE 290
//*                                                                 *   FILE 290
//*           SECURE:   MVS integrity is maintained.  if an         *   FILE 290
//*           authorized program opens a GPSAM file, the "access    *   FILE 290
//*           method" module is limited to those explicitly         *   FILE 290
//*           permitted by an installation-supplied name table      *   FILE 290
//*           and the module must come from an APF library.         *   FILE 290
//*                                                                 *   FILE 290
```
