# How-to-launch-jenkins-install-centos-docker

First download the jenkins docker images using below command.

`docker pull bitroid/centosjenkins:latest`

and run below command to run jenkins docker in detached mode.

`docker run -d --privileged -p 8080:8080 bitroid/centosjenkins:latest`

after executing above command jenkins will running in `localhost:8080` or `127.0.0.1:8080`.  
If you are using server with private then `private_ip_address:8080`.

_**Credentials**_

_Username:_ **admin**  
_Password:_ **admin**

**Badges**

[![](https://images.microbadger.com/badges/image/bitroid/centosjenkins.svg)](https://microbadger.com/images/bitroid/centosjenkins)

[![](https://images.microbadger.com/badges/version/bitroid/centosjenkins.svg)](https://microbadger.com/images/bitroid/centosjenkins)

