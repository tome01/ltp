#
# Read COPYING for licensing details.
#
# Ngie Cooper, June 2010
#

all clean install test:
	@for dir in `ls -d */Makefile 2>/dev/null | sed -e 's,/Makefile$$,,g'`; do \
		$(MAKE) -C $$dir $@;						   \
	done

distclean-makefiles:
	@find */ -name 'Makefile*' | grep -v threads/Makefile | grep -v timers/Makefile | xargs rm -f
