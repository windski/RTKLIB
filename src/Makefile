CC = gcc
AR = ar
CCFLAGS = -O2
ARFLAGS = rcs
OBJS = convkml.o convrnx.o datum.o download.o ephemeris.o geoid.o ionex.o lambda.o\
	options.o pntpos.o postpos.o ppp_ar.o ppp.o preceph.o qzslex.o rcvraw.o rinex.o\
	rtcm.o rtcm2.o rtcm3.o rtcm3e.o rtkcmn.o rtkpos.o rtksvr.o sbas.o solution.o\
	stream.o streamsvr.o tle.o

all: $(OBJS)
	$(AR) $(ARFLAGS) librtk.a $(OBJS)

.c.o:
	$(CC) $(CCFLAGS) -c $< -o $*.o

clean:
	rm -f *.o *.a
