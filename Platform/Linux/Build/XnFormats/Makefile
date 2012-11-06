SRC_FILES = \
			../../../../Source/XnFormats/*.cpp

LIB_NAME = XnFormats
USED_LIBS = XnCore OpenNI
DEFINES = XN_FORMATS_EXPORTS

ifeq ($(shell ld -ljpeg -o /dev/null 1>&2 2> /dev/null; echo $$?), 0)
  USED_LIBS += jpeg
else
  INC_DIRS  += ../../../../Source/External/LibJPEG
  SRC_FILES += ../../../../Source/External/LibJPEG/*.c
endif

include ../EngineLibMakefile
