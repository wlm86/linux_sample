obj-m += kthread.o

KERNELDIR := /lib/modules/$(shell uname -r)/build
PWD := $(shell pwd)
all:
	$(MAKE) -C $(KERNELDIR) M=$(PWD) modules

clean:
	rm -rf *.ko *.mod* *.o modules.* Module.symvers

install:
	insmod kthread.ko

remove:
	rmmod kthread
