if HAVE_FT12
FT12 = ft12.h ft12.cpp lowlatency.h lowlatency.cpp
else
FT12 =
endif

if HAVE_PEI16s
PEI16s = bcu1serial.h bcu1serial.cpp lowlatency.h lowlatency.cpp
else
PEI16s =
endif

if HAVE_TPUARTs
TPUARTs = tpuartserial.h tpuartserial.cpp lowlatency.h lowlatency.cpp
else
TPUARTs =
endif

if HAVE_EIBNETIP
EIBNETIP = eibnetrouter.h eibnetrouter.cpp
else
EIBNETIP =
endif

if HAVE_EIBNETIPTUNNEL
EIBNETIPTUNNEL = eibnettunnel.h eibnettunnel.cpp
else
EIBNETIPTUNNEL =
endif

if HAVE_USB
USB = usbif.h usbif.cpp
else
USB =
endif

if HAVE_NCN5120
NCN5120 = ncn5120.h ncn5120.cpp
else
NCN5120 = 
endif

noinst_LIBRARIES = libbackend.a
AM_CPPFLAGS=-I$(top_srcdir)/src/libserver -I$(top_srcdir)/src/common -I$(top_srcdir)/src/usb $(PTH_CFLAGS) $(LIBUSB_CFLAGS)

libbackend_a_SOURCES= $(FT12) $(PEI16s) $(TPUARTs) $(EIBNETIP) $(EIBNETIPTUNNEL) $(USB) $(NCN5120) dummy.cpp

