# Secure_SOXFire
Information publishing platforms are very important currently because there are many and various data on all over the world by become popular IoT. 
Like this, exceeding smart cities have happened the extreme generating data there.  
In these backgrounds, we must prepare the platform to publish data efficiently to multiple clients.
Publish/Subscribe messaging model(Pub/Sub model) is thought to suit as IoT data platform because this model can realize to push and broadcast data to many clients.

<img width="1426" alt="pubsub" src="https://user-images.githubusercontent.com/13267712/140929993-213ef2e7-2e85-4967-a067-e7412e594402.png">


SOXFire is implemented by extended Openfire(https://www.igniterealtime.org/projects/openfire/).
Openfire is the open-source instant massaging platform based on XMPP.
SOXFire is extended for managing sensor data.
If you want to publish data from the complex sensor, you can realize it easily by using SOXFire.
The feature is shown in the following images.

We use this to realize data streaming to various situations in the M-Sec project.
<img width="1426" alt="soxfire" src="https://user-images.githubusercontent.com/13267712/140930183-0af6e836-fc05-4b0e-9fc3-66e2416288d1.png">



## Installation
### use Docker
install docker

edit docker-compose.yml and change password (suggested) and ports (if necessary)
open a terminal and change the workdir to ./soxfire

#### create images
run  docker-compose build

#### start service
run docker-compose up

initialize soxfire via webgui at http://[host-name]:9090
following the 3.Configuration at https://sox.ht.sfc.keio.ac.jp/soxfire/index.html
POINT:  set the host-name to "dbserver" in the database configure
