Requeriments:
=============

* Python 2.6.6 or more.
* Install Oracle Instant Client Basic RPM Package.
* Install cx_Oracle Module for python  ( http://cx-oracle.sourceforge.net )
* Create ldconfig file in /etc/ldconfig/oracle.conf with the oracle client lib path. 
	( In my case: /usr/lib/oracle/11.2/client64/lib)

Issues detected
===============

When the script tries to import de cx_Oracle library the system reports errors like: 
ImportError: libclntsh.so.11.1: cannot open shared object file: No such file or directory

Fix: create oracle.conf file with the correct path inside.

More: http://www.programmers-pain.de/2011/07/10/howto-install-cx-oracle-on-centos-5-x/
