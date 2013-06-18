svn2git
=======

SVN to git conversion for pywikibot. This is a shallow and modified
copy of the WMF svn2git operations repository [1]. Their svn2git is
based on the original work by Thiago Macieira and Thomas Zander,
with modifications and scripts by Chad Horohoe.

[1] https://git.wikimedia.org/summary/operations%2Fsoftware.git

Requirements
------------
 * working c++ compiler
 * libsvn-dev
 * libqt-dev (?)
 * 

Building
--------
``` bash
# build svn2git
qmake
make

# 
cd scripts-pwb
make # or make output/pywikiparser, make output/pywikipedia, etc.
```
