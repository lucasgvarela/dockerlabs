```
docker run myimage # result: "cat /etc/passwd" and "cat /etc/hosts"
docker run myimage /etc/resolv.conf # will override the CMD arguments and will "cat /etc/resolv.conf"
```