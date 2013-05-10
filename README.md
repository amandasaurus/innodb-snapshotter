innodb-snapshotter runs in the terminal and will take a copy of your
``INFORMATION_SCHEMA.INNODB_*`` tables for later analysis.

By default it takes copies of the tables ``INNODB_TRX``, ``INNODB_LOCKS`` and
``INNODB_LOCK_WAITS``. It takes a snapshot every 10 seconds. This can be
changed with the ``-d`` (delay) flag.

If you are running some load/performance testing, which has a bottleneck in
MySQL, this programme, and these snapshots can help you diagnose the problem
after the fact.

Copyright 2013, Rory McCann <rory@technomancy.org>, Released under GNU GPL
version 3, or at your option, a later version. See the file LICENCE for more.
