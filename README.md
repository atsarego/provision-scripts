# How to ssh to vagrant
> ssh -F vagrant/vagrant-ssh vagrant-node

# To run provision need to create hosts file
## Example:
>[all]  
>host1  
>host2  
>  
>[all:vars]  
>ansible_user=some_user  
>docker_registry=host1  
>
>[docker_nodes]  
>host1  
>host2  
>  
>[docker_registry]  
>host1