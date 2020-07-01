wsl-tips

## X Server
VcxSrv:
* install [VcxSrv](https://sourceforge.net/projects/vcxsrv/)
* find XLauch on windows menu, and start server, for WSL2 flag "Disable access controll"

for WSL1 on .bashrc or .zshrc
```sh
export DISPLAY=:0.0 
```

for WSL2
```
# Get the IP address of the host from /etc/resolv.conf
export WSL_HOST=$(tail -1 /etc/resolv.conf | cut -d' ' -f2)
# Set the display path
export DISPLAY=$WSL_HOST:0.0
```

for hight DPIs
```
export GDK_SCALE=0.5   
export GDK_DPI_SCALE=1.25 
```
