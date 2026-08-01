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


Zipping and unzipping
-----------------------
rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude$ zip -r test_dir.zip test_dir
  adding: test_dir/ (stored 0%)
  adding: test_dir/renamed_example.txt (stored 0%)
rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude$ ls
README.md  test_dir  test_dir.zip
rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude$ unzip -l test_dir.zip unzipped.dir
Archive:  test_dir.zip
  Length      Date    Time    Name
---------  ---------- -----   ----
---------                     -------
        0                     0 files
rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude$ ls
README.md  test_dir  test_dir.zip
rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude$ unzip test_dir.zip -d unzipped_dir
Archive:  test_dir.zip
   creating: unzipped_dir/test_dir/
 extracting: unzipped_dir/test_dir/renamed_example.txt  
rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude$ ls
README.md  test_dir  test_dir.zip  unzipped_dir
rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude$ 

Downloading files
-------------------
rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude$ wget https://example.com/sample.txt
--2026-08-02 02:08:54--  https://example.com/sample.txt
Resolving example.com (example.com)... 2606:4700:9a95:72db:f2ef:694:ef6b:ff98, 104.20.23.154, 172.66.147.243
Connecting to example.com (example.com)|2606:4700:9a95:72db:f2ef:694:ef6b:ff98|:443... connected.
HTTP request sent, awaiting response... 404 Not Found
2026-08-02 02:08:55 ERROR 404: Not Found.


Changing Permissions
--------------------
Created a file named "secure.txt" using touch command and changed the permissions 
4 (Owner): Read (r--)
4 (Group): Read (r--)
4 (Others): Read (r--)

rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude$ chmod 444 secure.txt

rohan-bhowmik@rohan-bhowmik-VMware-Virtual-Platform:~/Documents/Linux_Assignment_Tutedude$ ls -al
total 28
drwxrwxr-x 5 rohan-bhowmik rohan-bhowmik 4096 Aug  2 02:12 .
drwxr-xr-x 5 rohan-bhowmik rohan-bhowmik 4096 Aug  2 01:41 ..
drwxrwxr-x 8 rohan-bhowmik rohan-bhowmik 4096 Aug  2 02:10 .git
-rw-rw-r-- 1 rohan-bhowmik rohan-bhowmik 3000 Aug  2 02:10 README.md
-r--r--r-- 1 rohan-bhowmik rohan-bhowmik    0 Aug  2 02:12 secure.txt
drwxrwxr-x 2 rohan-bhowmik rohan-bhowmik 4096 Aug  2 01:47 test_dir
-rw-rw-r-- 1 rohan-bhowmik rohan-bhowmik  352 Aug  2 02:02 test_dir.zip
drwxrwxr-x 3 rohan-bhowmik rohan-bhowmik 4096 Aug  2 02:04 unzipped_dir




