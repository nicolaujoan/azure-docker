# azure-docker 🖥️ 🐳

### Intro:

We are gonna create a Debian VM in Azure and the connect it through SSH protocol with our local machine. Then we will install docker and git on it.

<hr>

### Quick refresher:

Let's refresh some SSH concepts:

- SSH is an encripted connection protocol

- Have secure sign-ins over unsecured connections

- Is the default connection protocol for linux VMs

- Is recommended by Microsoft to connect to a VM over SSH keys (public-private key pair)
    - public key -> on linux VM
    - private key -> on local system

<hr>

### VM creation:

![1-create](./imgs/1-create.png)

First we click on create VM

![2-features](./imgs/2-vm_feat.png)

then select the features of our machine

![3-ssh](./imgs/3-ssh_keys.png)

select the ssh keys

![4-disk](./imgs/4-disk.png)

Our disk characteristics

![5-review](./imgs/5-review_create.png)

Create our machine

![6-keypair](./imgs/6-generate_keypair.png)

generate keypair

![7-downloadkeypair](./imgs/7-download_keypair.png)

download key pair

![8-vmsucces](./imgs/8-vm_succeed.png)

vm created with success


![9-connect](./imgs/9-connect_apartado.png)

Due to technical problems we connect with a password instead of ssh keypair. SO we proceed and get the public ip address of the VM

![11-publicip](./imgs/11-public-ip.png)

execute the following command to start the connection

![12-connection](./imgs/12-connection.png)

now that are connected, we install git

![git](./imgs/git_instal.png)

check for its version

![git--version](./imgs/git_version.png)

Now we are ready to install docker, but in ninja mode

![docker_install](./imgs/13-docker_install.png)

check for its version

![docker-v](./imgs/14-docker_version.png)

Now we are ready to dockerize our app, so do a clone from our github repo

![clone](./imgs/15-repo.png)

![clone-2](./imgs/16-clone.png)

ready to build

![build](./imgs/17-docker_build.png)

build success

![ready](./imgs/19.build_succes.png)

finally, run the container

![run](./imgs/20_docker_run.png)







