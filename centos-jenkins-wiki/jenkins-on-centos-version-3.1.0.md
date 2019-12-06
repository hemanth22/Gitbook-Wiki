# Jenkins-on-CentOS-version-3.1.0

First download the jenkins docker images using below command.

`docker pull bitroid/centosjenkins:release-3.1.0`

and run below command to run jenkins docker in detached mode.

`docker run -d --privileged -p 8080:8080 bitroid/centosjenkins:release-3.1.0`

or

Execute below docker command only if is create with filename: /opt/jenkins, if not create a foldername: /opt/jenkins and execute the command.

`docker run -d --privileged -p 8080:8080 --volume="/opt/jenkins:/var/lib/jenkins:rw" --name jenkins bitroid/centosjenkins:release-3.1.0`

after executing above command jenkins will running in `localhost:8080` or `127.0.0.1:8080`.  
If you are using server with private then `private_ip_address:8080`.

**Credentials**

_Username:_ **admin**  
_Password:_ **admin**

**New feature:**

* Added docker-compose. 
* configured docker access.   
* Bcrypt.  

**How to test this image in play with docker.**

Use below command to download jenkins and follow the instructions.

`wget -O- https://git.io/JenkinsDInD | sh`

