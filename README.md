# Linux_Assignment_Tutedude
Regarding Linux Basics Assignment

Viewing File Contents
-----------------------------

rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude/test_dir$ cat /etc/passwd | head -n 5
root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync

rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude/test_dir$ cat /etc/passwd | tail -n 5
gnome-initial-setup:x:119:65534::/run/gnome-initial-setup/:/bin/false
gdm:x:120:121:Gnome Display Manager:/var/lib/gdm3:/bin/false
nm-openvpn:x:121:122:NetworkManager OpenVPN,,,:/var/lib/openvpn/chroot:/usr/sbin/nologin
rohan-bhowmik:x:1000:1000:Rohan Bhowmik:/home/rohan-bhowmik:/bin/bash
sshd:x:122:65534::/run/sshd:/usr/sbin/nologin


Searching patterns
----------------------
rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude/test_dir$ cat /etc/passwd | grep root
root:x:0:0:root:/root:/bin/bash
nm-openvpn:x:121:122:NetworkManager OpenVPN,,,:/var/lib/openvpn/chroot:/usr/sbin/nologin





