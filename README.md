Extractenator - a spicy self-extracting installer creator
====================================

Copyright 2018-2022 Michael D Labriola <veggiemike@sourceruckus.org>

Licensed under the GPLv3. See the file COPYING for details. 

Extractenator is a utility for creating compressed, self extracting
executables that run an embedded install script after extracting to a
temp directory.

Get the latest and greatest from https://github.com/sourceruckus/extractenator.

<pre>
usage: extractenator OPTIONS PAYLOAD...

  -f, --filename EXEFILE    Specify output filename. (REQUIRED)

  -e, --exclude PATTERN     Exclude files in PAYLOAD that match PATTERN,
                            a glob(3)-style wildcard pattern.  Can be
                            specified multiple times.

  -s, --script SCRIPT       Specify installation script to be run after
                            extraction.  SCRIPT will be included as archive
                            content, you don't have to also specify it as
                            payload. (REQUIRED)

  -c, --compressor COMP     Use COMP compressor in pipeline during archive
                            creation.  Valid compressors are 'gzip', 'bzip2',
                            'xz', 'zstd', or 'none'.  Default is 'zstd' w/
                            --compressor-args of -T0 -10.  If COMP is specified
                            as 'none', no compressor is used (e.g., if payload
                            files are already compressed).

  -C, --compressor-args ARGS  Pass ARGS into the specified compressor.  If
                              --compressor was specified, defaults to empty
                              string.  Otherwise, default is '-T0 -10' to go
                              along with the default zstd compressor.  Can be
                              provided multiple times, causing argurments to be
                              appended (i.e., becaue you cannot have spaces in
                              ARGS).
</pre>
