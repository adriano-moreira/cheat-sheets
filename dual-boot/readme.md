https://www.howtogeek.com/323390/how-to-fix-windows-and-linux-showing-different-times-when-dual-booting/

on ubuntu or linux with systemd
```sh
#show current config
timedatectl

#enable RTC in local TZ
timedatectl set-local-rtc 1 --adjust-system-clock
```
