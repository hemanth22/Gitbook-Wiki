# Jenkins-on-CentOS-version.

First download the jenkins docker images using below command.

`docker pull bitroid/centosjenkins:1`

and run below command to run jenkins docker in detached mode.

`docker run -d --privileged -p 8080:8080 -p 50000:50000 bitroid/centosjenkins:1`

after executing above command jenkins will running in `localhost:8080` or `127.0.0.1:8080`.  
If you are using server with private then `private_ip_address:8080`.

_**How to use the customized docker.**_

`docker run -d --privileged -p 8080:8080 --name jenkins bitroid/centosjenkins:latest`

_Username:_ **admin**  
_Password:_ **admin**

