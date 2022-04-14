# Source



First I started Nmap and discovered the use of `webmin version 1.890` on port `10000`<br>

<img src="https://i.imgur.com/EpFC00y.png"/>

I searched for an exploit and found a reverse shell on metasploit<br>

<img src="https://i.imgur.com/Y6KjzUG.png"/>

After I set the options I started the exploit and became `root` on the target system.<br>

<img src="https://i.imgur.com/VSGS2TP.png"/>

After executing `python -c 'import pty;pty.spawn("/bin/bash")'`, I was able to use the shell.

I found the flags as usual in the `/home` and `/root` directory