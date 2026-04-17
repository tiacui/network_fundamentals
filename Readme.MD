
1) Understand the URLs:

```
https://x.com/glevonian/status/2044432429746647041
```

- protocol: https                   #encrypted
- Host: ```x.com```
- route: ```/glevonian/status/2044432429746647041```
- parameter: ```2044432429746647041```


```
http://bb.im5.org/learning/lesson1.php?username=john&color=blue
```

- protocol: http                  # unencrypted
- Host: ```bb.im5.org```
- route: ```/learning/lesson1.php```
- parameter: ```username=john&color=blue```


2) Inspect the HTTP ```request & response```

- use Chrome "Developer Tool"
  - visit the URL in Chrome -> ```right click``` -> ```Inspect``` -> ```Network``` -> ```refresh``` -> check ```Response```, ```Preview```, ```Headers```

- use CURL
  - in ```cmd.exe``` -> run ```curl -i "http://bb.im5.org/learning/lesson1.php?username=john&color=blue"```
  - inspect the HTTP headers, HTTP body in the response



============================================

3), TCP ports test1

- use command ```netstat -an``` in cmd.exe to list open ports
- use ```python3 -m http.server 8111``` to start a simple http server and listen on port 8111        (can be any ports; "http.server" is a python module)
- use command ```netstat -an``` in cmd.exe to list open ports, and observe port 8111 listening
- vist ```http://localhost:8111``` via chrome
- use command ```netstat -an``` in cmd.exe to list open ports, and observe connections to port 8111 established

4), TCP ports test2

- in cmd.exe, run ```ssh test@192.168.1.102``` and enter password ```test123``` to logon 192.168.1.102 remotely
- run ```nc -l 4000``` to listen port port 4000 on ```192.168.1.102```
- in cmd.exe, run ```telnet 192.168.1.102 4000``` to connect to port 4000 on ```192.168.1.102```
- in the telnet window, enter random string and press enter, it can be observed the string shown in the remote windows of ```192.168.1.102```




