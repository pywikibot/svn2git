OPTS=--identity-map=authors.alias --svn-branches
SVNROOT=svnroot

all:
	echo Please define which project you want to export

svnroot:
	./sync

export:
	../svn-all-fast-export $(OPTS) --rules=total.rules $(SVNROOT)

push:
	cd output/core && git remote add origin https://github.com/pywikibot/core.git && git push -u -f origin master
	cd output/i18n && git remote add origin https://github.com/pywikibot/i18n.git && git push -u -f origin master
	cd output/compat && git remote add origin https://github.com/pywikibot/compat.git && git push -u -f origin master
	cd output/spelling && git remote add origin https://github.com/pywikibot/spelling.git && git push -u -f origin master

clean:
	rm -rf output/*
