#created by zhangwei on 2017-04-10

include ../makefilecommon.inc
OBJECTS=config.o
LOCALSTATICLIB=libconfig.a

all:$(LOCALSTATICLIB)

$(LOCALSTATICLIB):$(OBJECTS)
	$(ARCH) $(LOCALSTATICLIB) $(OBJECTS)
	rm *.o
$(OBJECTS):%.o:%.c
	$(CC) -c $(INCLUDE_PATH) $< -o $@

clean:
	rm $(LOCALSTATICLIB)

