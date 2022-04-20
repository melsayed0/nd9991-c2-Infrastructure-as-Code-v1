


For the review requirment:
I have added the below screenshoots which refelct the required change :
    1- EC2 Type Changed to t3.medium.png
    2- Web services is working fine.png


Table of content :

1- Submitter information.
2- URL for the dummy Web page 
3- Folder contents overview.
4- How to run the Project material?

For the review requirments:
I have added the below screenshoots which refelct the required change :


# 1- Submitter information:

    Mohamed Elsayed (ID:782943564937) / FWD Udacity 2nd Project.

# 2- URL for the project dummy Web page: 

    http://serve-webap-1g0pb1qp3x5ba-930863025.us-east-1.elb.amazonaws.com/

# 3- Folder contents overview :

    This Folder contains the main two project requiremnts :

        1- The Infrastructure Design Digram >>> 2ndproject-Drawing.JPG

        2- The cloudfomration Stacks deployment codes :

            a.Network Stack (Network-782943564937):
                i.Network template >>> CF-Network.yml
                ii.Netwrok Parameters >>> CF-Network_Parameters.json

            b.Servers Stack (Servers-782943564937):
                i.Servers template >>> CF-Servers.yml
                ii.Servers template >>> CF-Servers_Parameters.json

    In addition it also contains the required bash scripts to run the project files :
        1- Create-Stack.sh
        2- Update-Stack.sh
        3- Delete-Stack.sh

# 4- How to run the Project material?


```bash

'At the project folder /FWD-782943564937-2ndProject/ run the below bash commands :

Note: The project is up and runing now , if it is required to run it from scratch please change the order to delete the Servers stack 1st then the Netwrok stack.'  

# 1- Creat the Netwrok stack 

./Create-Stack.sh Network-782943564937 CF-Network.yml CF-Network_Parameters.json

# Note :We should wait for the Netwrok Stack to be Created sucssfully and resources are ready before launch the Servers Stack

# 2- Creat the Netwrok stack 

./Create-Stack.sh Servers-782943564937 CF-Servers.yml CF-Servers_Parameters.json

'After sucssful stacks creation we should be able to access the dummy web service from the loadbalancer DNS URL .
 we can access the loadbalancer URL from the Servers-782943564937 Stack output tap' 

# After Sucssful verfications we can release the resuources as below :

#  Delete the Servers Stack

./Delete-Stack.sh Servers-782943564937

# We should wait for the Netwrok Stack to be deleted sucssfully and resources released before delete the Servers Stack

#  Delete the Netwrok Stack

./Delete-Stack.sh Network-782943564937

```


