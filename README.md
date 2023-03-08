## Catalinul-ProgramingAssessment

This is a project used to showcase an assessment task where I had to create deployment scripts using Ansible to deploy an application to some target servers (or virtual
machines). The application that I had to deploy is [the ToDo app from Docker's website](https://docs.docker.com/get-started/02_our_app/). 


A video of the controller node with Ansible and the remote VM target [can be found here](https://youtu.be/5JlXS67otDc). 
Unfortunately, I didn't know where I can get an online VM from, in order to just share the link with it. I had to go with VirtualBox and classic VMs.

For both the Ansible VM and for the target VM I have used CentOS 7. I had this image lying around in my computer `CentOS-7-x86_64-DVD-2009`.
These are the settings that I installed the image with:
![setup vm screen](https://user-images.githubusercontent.com/22594116/223818846-cfac55ab-7197-431c-b877-fc4e863a9006.png)
It was the most basic and minimal installation I could, since I needed a GUI for accesing Firefox, in order to see the app runing.

The command I've used to run the playbook is:

```
sudo ansible-playbook start-app.yml -v
```


I've had to do some changes in the docker-compose file found in the Docker tutorial. I added this healthcheck:
```
 healthcheck:
      test: /usr/bin/mysql --user=root --password=secret --execute "SHOW DATABASES;"
 ```
 Without it, the app would sometimes crash. The mysql container would be running much sooner than the app's container. In this way, the app container only starts after the database can be querried.

The inventory is the hosts file. 





