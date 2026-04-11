# HLL_CRCON_Diagnose_file
If you encounter issues using Hell Let Loose (HLL) CRCON (see : https://github.com/MarechJ/hll_rcon_tool), you'll have to give technical informations about your installation if you want to receive some help or advice.
That means you would have to enter multiple commands in your VPS terminal. This can be rather long and techy.

-> This bash script will automatically collect all the debugging infos in a single file you can share with the person who is trying to help you.

### :warning: Sensitive data
- Please be careful about sharing this file, as it could contain your personal passwords (RCON, CRCON database, etc).  
The script should have (redacted) them, but... Just check OK ?
- **NEVER share it on a public forum / Discord channel** ;
- If you do not fully trust the person asking these informations, you can open the file with any text editor and delete any sensitive data before sharing (search in it for your passwords, VPS and game server IPs, etc).

---

## Install

> [!IMPORTANT]
> - The shell commands given below assume your CRCON is installed in `/root/hll_rcon_tool`  
>   You may have installed your CRCON in a different folder.  
>   If so, you'll have to adapt the commands below accordingly.
>
> - Always copy/paste/execute commands :warning: one line at a time :warning:

### 1/2 - Log into your CRCON host machine using SSH

- See [this guide](https://github.com/MarechJ/hll_rcon_tool/wiki/Troubleshooting-&-Help-‐-Common-procedures-‐-How-to-enter-a-SSH-terminal) if you need help to do it.

### 2/2 - Download file
```shell
cd /root/hll_rcon_tool
```
```shell
wget https://raw.githubusercontent.com/ElGuillermo/HLL_CRCON_Diagnose_file/refs/heads/main/diagnose.sh
```

---

## Use

### 1/2 - Log into your CRCON host machine using SSH

### 2/2 - Launch script

  ```shell
  cd /root/hll_rcon_tool
  ```
  ```shell
  sh ./diagnose.sh
  ```
- download the `/root/hll_rcon_tool/diagnose.log` file
- review its content for sensitive data
- share it
