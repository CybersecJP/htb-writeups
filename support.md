# Support

Support

* Target: 10.10.11.174
* HTB , Windows machine

#### Ping <a href="#ping" id="ping"></a>

* As we can see target is alive with "ttl=127" (probably a windows machine).

```
ping 10.10.11.174
```

```
ping 10.10.11.174
```

#### Nmap <a href="#nmap" id="nmap"></a>

```
nmap -T4 -A -v 10.10.11.174
```

```
nmap -T4 -A -v 10.10.11.174
```

#### crackmapexec <a href="#crackmapexec" id="crackmapexec"></a>

```
cme smb 10.10.11.174 -u 'anonymous' -p '' --rid-brute
```

```
cme smb 10.10.11.174 -u 'anonymous' -p '' --rid-brute
```

```
cat u.txt |grep -i user |rev |cut -f2 -d ' ' |rev |grep SUPPO |cut -f2 -d '\' |grep -Ev (DC|SVC) |tail -n +4 > users.txt
```

```
cat u.txt |grep -i user |rev |cut -f2 -d ' ' |rev |grep SUPPO |cut -f2 -d '\' |grep -Ev (DC|SVC) |tail -n +4 > users.txt
```

Result:\
