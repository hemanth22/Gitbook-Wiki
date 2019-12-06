# Bulter-common-error-troubleshooting-tips.

Hello user,

When you have below kind of errors, perform below troubleshooting tip.

```text
[root@12d21c4bf969 /]# butler plugins import --server http://localhost:8080/ --username admin --password admin
Installing jdk-tool@1.2
Not found 404
```

```text
[root@12d21c4bf969 /]# butler plugins import --server localhost:8080
Installing jdk-tool@1.2
Unauthorized 401
```

**Troubleshooting Steps.**

1. Go to jenkins homepage and go to Configure Global Security as below.  
2. From jenkins homepage &gt; **Manage Jenkins** &gt; **Configure Global Security**.  
3. Under Configure Global Security, search keyword : **CSRF Protection**.  and make configuration as shown in below screenshot and save it, this will resolve the issue.

![Troubleshooting.](https://i1311.photobucket.com/albums/s673/hemanth22hemu/CSRFProtection_zpshro9gk0h.jpeg)

