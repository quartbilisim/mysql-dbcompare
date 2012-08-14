# MySQL DBCompare

This commandline script will generate a structure diff of two input files and echo it to SDOUT.

It uses the "Database structure synchronizer" class from [phpclasses.org](http://www.phpclasses.org/package/4615-PHP-Compare-MySQL-databases-to-synchronize-structures.html) with a simple commandline interface. 

**Usage:**

```bash

# simple (no arguments)
$ ./dbcompare.php

# alternative (source files supplied as arguments)
$ ./dbcompare.php path/to/source.sql path/to/destination.sql

```

An example test script can be executed with:
```bash
$ ./dbcompare.php test/dev.sql test/live.sql
```

This script assumes your php runtime is located at `/usr/bin/php`, if it's not you'll need to change it at the top of the file. You could copy the script into `/usr/local/bin` and rename it to `dbcompare` to make usage simpler.

