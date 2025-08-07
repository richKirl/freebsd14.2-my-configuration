# freebsd14.2-my-configuration
freebsd14.2 my configuration

MYKERNEL - without RAID without nvme, with some stuff for terminal vt(4)



```
##########################################
#cd /usr/src/sys/amd64/conf              #
#                                        #
#mkdir /root/kernels
#                                        #
#cp GENERIC /root/kernels/MYKERNEL
#                                        #
#ln -s /root/kernels/MYKERNEL
#                                        #
##########################################
##some edit kernel########################
##########################################
#                                        #
#cd /usr/src/sys/amd64/conf && make LINT #
#                                        #
#cd /usr/src                             #
#make buildkernel KERNCONF=MYKERNEL      #
#                                        #
#make installkernel KERNCONF=MYKERNEL    #
##########################################
#                                        #
#shutdown -r now                         #
##########################################
```




resources

```docs.freebsd.org/en/books/handbook/x11/```

```zenarmor.com/docs/freebsd-tutorials/how-to-configure-freebsd-kernel```
