OPTS=--identity-map=authors.alias --svn-branches
SVNROOT=svnroot

all:
	echo Please define which project you want to export

svnroot:
	./sync

output/pywikiparser:
	../svn-all-fast-export $(OPTS) --rules=parser.rules $(SVNROOT)

output/pywikipedia:
	../svn-all-fast-export $(OPTS) --rules=pwb.rules $(SVNROOT)
