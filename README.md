## Catalinul-ProgramingAssessment

This is a project used to showcase an assessment task where I had to create deployment scripts using Ansible to deploy an application to some target servers (or virtual
machines). The application that I had to deploy is [the ToDo app from Docker's website](https://docs.docker.com/get-started/02_our_app/). 


A video of the controller node with Ansible and the remote VM target [can be found here](https://youtu.be/5JlXS67otDc). 
Unfortunately, I didn't know where I can get an online VM from, in order to just share the link with it. I had to go with VirtualBox and classic VMs.

For both the Ansible VM and for the target VM I have used CentOS 7. I had this image laying around my computer `CentOS-7-x86_64-DVD-2009`.


The command I've used to run the playbook is:

```
sudo ansible-playbook start-app.yml -v
```



