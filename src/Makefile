#src Makefile

include ../Makefile.common
program=$(PROGRAM).a
objs=$(patsubst %.c,%.o,$(wildcard *.c))

all: src
src: $(program)

$(program): $(objs)
	$(AR) cr $@ $(objs)

.PHONY: src clean tshow

clean:
	rm -f $(program) $(objs)

tshow:
	@echo "###################################################################    ###################################"
	@echo "################# optimize settings: $(InfoTextLib), $(InfoTextSrc)    "
	@echo "###################################################################    ###################################"

