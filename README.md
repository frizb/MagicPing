# MagicPing
Python 2.7 raw socket ICMP ping to send a embedded message or a magic ping to an endpoint.

# Usage 
verbose_ping( <ip address>, <timeout seconds>, <number of pings to send>, <message to embed in data>)

# Testing
verbose_ping('192.168.218.1',2,4,'Hello From Ping!!!!!!!!!!!!!!!!!')


0000   00 50 56 c0 00 08 00 0c 29 25 75 dc 08 00 45 00  .PV.....)%u...E.
0010   00 38 c8 35 40 00 40 01 3c ba c0 a8 da 82 c0 a8  .8.5@.@.<.......
0020   da 01 08 00 95 a3 70 84 01 00 48 45 4c 4c 4f 20  ......p...HELLO 
0030   46 52 4f 4d 20 50 49 4e 47 21 21 21 21 21 21 21  FROM PING!!!!!!!
0040   21 21 21 21 21 21                                !!!!!!


 Modified from the original source found here:
    https://gist.github.com/pklaus/856268


    Other Repositories of python-ping
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    * https://github.com/l4m3rx/python-ping      supports Python2 and Python3
    * https://bitbucket.org/delroth/python-ping
    About
    ~~~~~
    A pure python ping implementation using raw socket.
    Note that ICMP messages can only be sent from processes running as root.
    Derived from ping.c distributed in Linux's netkit. That code is
    copyright (c) 1989 by The Regents of the University of California.
    That code is in turn derived from code written by Mike Muuss of the
    US Army Ballistic Research Laboratory in December, 1983 and
    placed in the public domain. They have my thanks.
    Bugs are naturally mine. I'd be glad to hear about them. There are
    certainly word - size dependenceies here.
    Copyright (c) Matthew Dixon Cowles, <http://www.visi.com/~mdc/>.
    Distributable under the terms of the GNU General Public License
    version 2. Provided with no warranties of any sort.
    Original Version from Matthew Dixon Cowles:
      -> ftp://ftp.visi.com/users/mdc/ping.py
    Rewrite by Jens Diemer:
      -> http://www.python-forum.de/post-69122.html#69122
    Rewrite by Johannes Meyer:
      -> http://www.python-forum.de/viewtopic.php?p=183720
