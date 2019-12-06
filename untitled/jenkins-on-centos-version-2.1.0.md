# Jenkins-on-CentOS-version-2.1.0

First download the jenkins docker images using below command.

`docker pull bitroid/centosjenkins:release-2.1.0`

and run below command to run jenkins docker in detached mode.

`docker run -d --privileged -p 8080:8080 bitroid/centosjenkins:release-2.1.0`

after executing above command jenkins will running in `localhost:8080` or `127.0.0.1:8080`.  
If you are using server with private then `private_ip_address:8080`.

**Credentials**

_Username:_ **admin**  
_Password:_ **admin**

**New feature:**

Docker in Docker for jenkins docker image.

