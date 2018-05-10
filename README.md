# Docker-in-docker command

#docker commands to run wit in container using host docker


docker run -d -v /var/run/docker.sock:/var/run/docker.sock -v /usr/bin/docker:/usr/bin/docker:ro -v /lib64/libdevmapper.so.1.02:/usr/lib/x86_64-linux-gnu/libdevmapper.so.1.02 -v /lib64/libudev.so.0:/usr/lib/x86_64-linux-gnu/libudev.so.0 -p 8080:8080 --name jenkins -u root --privileged=true -t -i bhargavbunny94/jenkins-bhargav


# TO SET A NAMESPACE AS DEFAULT NAMESPACE IN KUBERNETES

kubectl config set-context $(kubectl config current-context) --namespace=flappybird-namespace
