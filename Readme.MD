
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
