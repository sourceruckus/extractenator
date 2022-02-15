Extractenator - a spicy self-extracting installer creator
====================================

Copyright 2018-2022 Michael D Labriola <veggiemike@sourceruckus.org>

Licensed under the GPLv3. See the file COPYING for details. 

Extractenator is a utility for creating compressed, self extracting
executables that run an embedded install script after extracting to a
temp directory.

Get the latest and greatest from https://github.com/sourceruckus/extractenator.

<pre>
usage: doit OPTIONS CMD...

  -f, --filename LOGFILE    Specify output filename.  Both stdout and stderr
                            will be redirected to this file.  When the process
                            finishes, the files last few lines will contain
                            "DOIT: ALL DONE", a return code, and timing stats.

  -m, --mail EMAILADDRESS   Email stdout/stderr to specified address instead
                            of logging to a file.

  -V, --version             Show version string and exit.
</pre>
