# Create VM in Azure 

```

az vm create --resource-group sidgs --name k8snode001 --image UbuntuLTS --admin-username ubuntu --ssh-key-value "Equifax\aws\kops_public"

az vm create --resource-group sidgs --name k8snode002 --image UbuntuLTS --admin-username ubuntu --ssh-key-value "Equifax\aws\kops_public"

az vm create --resource-group sidgs --name k8smaster --image UbuntuLTS --admin-username ubuntu --ssh-key-value "Equifax\aws\kops_public"

az vm create --resource-group sidgs --name k8scontroller --image UbuntuLTS --admin-username ubuntu --ssh-key-value "Equifax\aws\kops_public"

```

# setup the inventory file 

- Get the IP Addresses  of the VM's 
- Got to the VM named k8scontroller 
- Login witu user 'ubuntu' and the key used to create this VM 
- Git clone this repo
- Follow instructions in the [readme](../../readme.md) file 
