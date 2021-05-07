# ansible-role-keepalived
Role to deploy keepalived in Kubernetes

## Vars
    
    keepalived_ns : namespace where to install keepalived
    keepalived_interface : interface where the vip will stand.
    keepalived_vip : the virtual ip  
      
## Tasks
A simple task that create the namespace and retrieve the manifest from [goacid/k8s_keeplived](https://github.com/goacid/k8s_keepalived) , sed vars and then deploy it.  
This manifest import a [docker image](https://hub.docker.com/r/goacid/keepalived): build for ARM64 only 
