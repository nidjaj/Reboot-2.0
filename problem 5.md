## play with files and directories 
### Problem

1.Create  3 files named   abc.txt  ok  fine  g.txt  /tmp directory  
2.Create  4  directories   aa aaa aaaa  under  /tmp directory  
3.Give ls command to  list the content of  /tmp directory  
4.Make sure it will only list the content (file|directory)  having 2 char in their name. 
### Solution 
 ```
[nidhijajoo@localhost ~]$ cd /tmp
[nidhijajoo@localhost tmp]$ touch abc.txt ok fine  g.txt
[nidhijajoo@localhost tmp]$ mkdir a aa aaa aaaa
[nidhijajoo@localhost tmp]$ ls
a
aa
aaa
aaaa
abc.txt
fine
g.txt
ok
systemd-private-00616fc305484880b16cdc38ed9809ca-chronyd.service-GmKc6i
systemd-private-00616fc305484880b16cdc38ed9809ca-colord.service-nz09cf
systemd-private-00616fc305484880b16cdc38ed9809ca-dbus-broker.service-Ybimcj
systemd-private-00616fc305484880b16cdc38ed9809ca-earlyoom.service-sVoetg
systemd-private-00616fc305484880b16cdc38ed9809ca-geoclue.service-ryVxoh
systemd-private-00616fc305484880b16cdc38ed9809ca-ModemManager.service-CNlgNg
systemd-private-00616fc305484880b16cdc38ed9809ca-rtkit-daemon.service-c1RzRg
systemd-private-00616fc305484880b16cdc38ed9809ca-switcheroo-control.service-v4n8qg
systemd-private-00616fc305484880b16cdc38ed9809ca-systemd-logind.service-bAZxag
systemd-private-00616fc305484880b16cdc38ed9809ca-upower.service-gNDZch
tracker-extract-files.1000
[nidhijajoo@localhost tmp]$ ls -d ??
aa  ok
[nidhijajoo@localhost tmp]$ 
```
