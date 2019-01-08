# Testing BANG

Testing BANG is important to find regressions. Currently there are two kinds of tests:

1. unit tests for individual files. These tests can be found inside the BANG repository. The test files are found in the directory 'test'. The script to test these is src/bangtest.py
2. regression tests with a large collection of firmware files. This is run regularly (every few weeks) to find any crashes or other odd behaviour. The firmware collection cannot be redistributed freely, so has not been made available.

## Notes

Some several notes which can be useful.

### Batch mode

To scan large amounts of files it is best to use the '-d' flag to BANG to scan lots of files, and to set "removescandirectory" in the configuration file to "yes".

### ext2

For ext2 a good set of testing data can be found in the e2fsprogs Git repository:

https://git.kernel.org/pub/scm/fs/ext2/e2fsprogs.git/tree/tests

### PNG/JPEG/GIF

Wikipedia's dumps in ZIM format possibly contain lots of pictures made with many different programs.