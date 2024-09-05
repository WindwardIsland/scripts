<h1 align="center">WindwardIsland/scripts</h1>

These are a collection of shell scripts that I either wrote myself, or took from others and modified them to fit my needs.

Feel free to poke around in here and see what scripts might be useful to you.

Note that most of the scripts that I wrote or taken from others, have been modified to be *strictly* POSIX-compliant. This means that these scripts don't use [bash](https://www.gnu.org/software/bash/) to read, interpret, and run them, but rather a strict POSIX-compliant, fast, and lightweight shell called [dash](http://gondor.apana.org.au/~herbert/dash/). This is denoted at the top of every script in this repository with the `#!/bin/sh` shebang (which is symlinked to `dash` by default on most Linux distributions, although the default is `bash` in Arch and Fedora) instead of a shebang like `#!/bin/bash` or `#!/usr/bin/env bash`. 

Using dash instead of bash is better to run scripts, because as stated earlier, dash is the default symlinked shell to `#!/bin/sh` on most Linux distributions, hence making them more portable and accessible to people on Linux that want to use these scripts. Note that there are some scripts in here that I unfortunately couldn't convert to be strictly POSIX-compliant due to some useful bashisms in those scripts (such as arrays), which is why I used the `#!/usr/bin/env bash` shebang for those scripts instead of `#!/bin/sh`.

Please also note that I have wrote these scripts on a Linux system, hence they are most likely to run successfully on one. I have not tested these scripts on alternative operating systems, such as macOS and the BSD family, so you are more than welcome to take these scripts and modify them to run successfully on those operating systems.

You should also run these scripts at your own risk! I am not responsible for any damage to your computer caused by running these scripts, so please be familiar with shell scripting before running these in order to understand what they actually do.

**NOTE**: I am planning to add a full description list at the bottom of every script in this repository soon, so please be patient!
