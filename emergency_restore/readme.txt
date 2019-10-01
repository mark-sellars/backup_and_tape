===========
Tape Backup
===========

Author
======

Mark R Sellars

About
=====

The contents of these tapes are compressed and archived by burp (BackUp Restore    
Program) then written to tape with TAR.I recommend installing centos or redhat 
then install burp-server and burp-client to restore the data from these tapes 
on a new server.

I have included a directory in these tapes called "emergency_restore". In this
directory everything you need to read the tape files, start a new backup
server, or restore the original backup server. Also included are the 
instructions on how to use these tapes and the software used for this tape library. 

Contents of emergency restore
=============================

| emergency_restore/
| ├── burp-git-clone
| ├── clientconfdir
| ├── images_vms
| │   ├── clonezilla
| │   │   └── burp-img
| │   └── kvm
| │       └── burp.qcow2
| ├── man_pages
| │   ├── burp_manpage.txt
| │   ├── mt_manpge.txt
| │   ├── mtx_manpage.txt
| │   ├── st_manpage.txt
| │   └── tar_manpage.txt
| ├── readme.txt
| ├── restoring_files.txt
| ├── restoring_sever_image.txt
| ├── scripts
| │   ├── chgtap
| │   └── tapebu
| └── tape_manual.txt

Getting Started
===============

 - How to read this tape set read "tape_manual.txt"

 - To restore tape files and install backup software read "restoring_files.txt"

 - To restore the original backup server read "restoring_server_image.txt"

 - Install backup software from source refer to documents in "burp-git-clone"

Information about these tapes
=============================

 - These tapes are LTO6

 - The data was backed up using BURP (Backup restore program)

 - These tapes should be in order of the numbers on them

 - The original server CPU: Intel Xeon E5-1620 V4

 - The original server operating system: Centos 7.6 64bit

 - All files written simply with TAR uncompressed. (No z Flag)
   - TAR cannot use compression on multi tape archives
