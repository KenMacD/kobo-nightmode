LINUX_PATH = /home/david/builds/kobo/linux-2.6.35.3-507
GCC = arm-linux-gnueabihf-gcc
INIPARSER = iniParser/iniparser.c iniParser/dictionary.c 

all:
	$(GCC) -I $(LINUX_PATH)/include -Wall -shared -ldl -fPIC -std=c99 -pthread -o screenInv.so screenInv.c $(INIPARSER)

debug:
	$(GCC) -I $(LINUX_PATH)/include -Wall -shared -ldl -fPIC -std=c99 -pthread -D SI_DEBUG -o screenInv.so screenInv.c $(INIPARSER)
