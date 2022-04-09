
Mohamed Elsayed (ID:782943564937) / FWD Udacity 2nd Project

### How to run the Project material?
We can run the project material in two easy steps:
```bash

# At the project folder /FWD-782943564937-2ndProject/ run the below bash commands in the below sequense

# 1- Creat the Netwrok stack 

./Create-Stack.sh Network-782943564937 CF-Network.yml CF-Network_Parameters.json

# We should wait for the Netwrok Stack to be Created sucssfully and resources are ready before launch the Servers Stack
# 2- Creat the Netwrok stack 

./Create-Stack.sh Servers-782943564937 CF-Servers.yml CF-Servers_Parameters.json

# After sucssful stacks creation we should be able to access the dummy web service from the loadbalancer DNS URL .
# we can access the loadbalancer URL from the Servers-782943564937 Stack output tap 

# After Sucessful verfications we can release the resuources as below :

#  Delete the Servers Stack

./Delete-Stack.sh Servers-782943564937

# We should wait for the Netwrok Stack to be deleted sucssfully and resources released before delete the Servers Stack

#  Delete the Netwrok Stack

./Delete-Stack.sh Network-782943564937

```


