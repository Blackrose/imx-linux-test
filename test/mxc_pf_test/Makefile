# list of platforms which did not want this test case
#EXCLUDE_LIST:="IMX27ADS IMX37_3STACK IMX51 IMX25_3STACK IMX6Q IMX6SL IMX6SX IMX7D IMX6UL"
INCLUDE_LIST:="IMX31 IMX53"

ifeq ($(PLATFORM),$(findstring $(PLATFORM),$(INCLUDE_LIST)))
OBJS = $(OBJDIR)/autorun-pf.sh $(OBJDIR)/mxc_pf_test.out
else
OBJS =
endif

all : $(OBJS)

.PHONY: clean
clean :
	rm -f $(OBJS)

#
# include the Rules
#
include ../make.rules

