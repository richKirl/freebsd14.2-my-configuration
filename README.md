# freebsd14.2-my-configuration
freebsd14.2 my configuration

<img width="1920" height="1050" alt="image" src="https://github.com/user-attachments/assets/b53ff698-a7a0-4c26-9819-96c3117ca324" />




MYKERNEL - without RAID without nvme, with some stuff for terminal vt(4)



```
##########################################
#cd /usr/src/sys/amd64/conf              #
#                                        #
#mkdir /root/kernels                     #
#                                        #
#cp GENERIC /root/kernels/MYKERNEL       #
#                                        #
#ln -s /root/kernels/MYKERNEL            #
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

install nvidia-drm drm-kmod x86-intel vdpau sdl2 sdl3 gnome nvidia 

nvidia-xconfig --prime

for debug - off lightdm_enable="NO" reboot



resources

```docs.freebsd.org/en/books/handbook/x11/```

```zenarmor.com/docs/freebsd-tutorials/how-to-configure-freebsd-kernel```
