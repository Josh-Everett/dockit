# dockit
This is a repo used for testing applications in an OpenShift/Kubernetes environment.

## Commands

```bash
sudo docker build -t flask-sample-one:latest .
sudo docker run -d -p 5000:5000 flask-sample-one 
```


Change the config/linux_env_vars to reflect an active interface
in my case
wlp4s0


```bash
oc whoami

oc get scc
oc adm -h
oc adm policy add-scc-to-user anyuid admin
oc get pods


oc create -f flask_pod.yml
oc create -f flask_services.yml

oc get pods
oc get ns
oc create ns testground
oc project testground

oc exec -it nginx-apparmor2 /bin/bash

oc describe service my-nginx

oc expose service my-nginx

oc get endpoints
oc get routes
```
