# ShellFind

## Description

```
Hello Hacker.
You don't know me, but I know you.
I want to play a game. Here's what happens if you lose.
The device you are watching is hooked into your Saturday and Sunday.
When the timer in the back goes off,
your curiosity will be permanently ripped open.
Think of it like a reverse bear trap.
Here, I'll show you.
There is only one UDP service to shell the device.
It's in the stomach of your cold firmware.
Look around Hacker. Know that I'm not lying.
Better hurry up.
Shell or out, make your choice.
```

## Run

```bash
sudo docker run --name shellfind -d --privileged -p 4444/udp --rm 1arry/shellfind
```

## Notes

1. You can find the raw Dockerfile at [here](https://drive.google.com/file/d/1uME-WEBL9cZGKcvsnQC0_jmRE_uSExUt/view?usp=sharing)
2. Please wait for ONE minute to start up
3. There is a THREE minutes timeout limit in raw competition challenge
4. Try to get an interactive shell, have fun! 

## Result

```
$ python exploit.py 192.168.5.128 49161 netcat
[*] Get mac address is 525400123456
[*] Send shellcode done
shell # ls
1
1>
2
2>
>
bin
dev
etc
etc_ro
firmadyne
home
lib
lost+found
mnt
mydlink
proc
rc.d
root
run
sbin
server
share
sys
tmp
usr
var
web

shell # ls firmadyne
busybox
console
debug.sh
dir_log
flag
gdb
gdbserver
libnvram
libnvram.override
libnvram.so
libnvram_ioctl.so
net_bridge
net_interface
network.sh
network_type
preInit.sh
run_service.sh
sh
strace
ttyS1

shell # cat /firmadyne/flag









rwctf{Find_udp_servic3_ORI_bind_U_h3r3_baby}
```
