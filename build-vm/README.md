## Build your own Virtual Machine

### Here's how you can spin up a Virtual Machine for tool Teamscale ...

#### Pre-requisites:  
1. Download and Install [Vagrant] (https://www.vagrantup.com/downloads.html)  
2. Download and Install [VirtualBox] (https://www.virtualbox.org/wiki/Downloads)  
3. Install [vagrant-reload] (https://github.com/aidanns/vagrant-reload) plugin using the command :  
    ```  
    $ vagrant plugin install vagrant-reload  
    ```  

#### Steps:  
1. Download all the files from [build-vm] () folder to the folder on your machine where you want to install the VM. Easiest way would be to git clone the repository and copy the contents of [build-vm] () folder to your VM folder :  
    ```  
    $ git clone https://github.com/SoftwareEngineeringToolDemos/ICSE-2014-Teamscale.git
    ```  
2. Navigate to VM installation folder (via bash on Linux or Command Prompt on Windows) and execute the command :  
    ```  
    $ vagrant up --provider virtualbox  
    ```  
3. Vagrant will start the VM and provision it. Please be patient as the VM will reload after provisioning completes.    

After VM is provisioned and it reloads :-  
    1. You will see Eclipse, a gnome-terminal and Firefox on startup.  
    2. On the terminal execute the command: 
        ```  
        $ sudo ./teamscale.sh  
        ```  
    3. On Firefox, refresh the tab :- `http://localhost:8080` (can take a few minutes to load).  
    4. Refer to the Readme.txt file on VM's Desktop for steps to run the tool.    

#### Note :   
 -  The vagrant reload plugin must be installed prior to running the "vagrant up" command.
 -  Vagrant provisioning may take upto 15-20 minutes. Please be patient.
 -  After provisioning completes the Virtual Machine will reboot but wait for the startup applications to load.  
 -  Default Virtual Machine Login Credentials:  
        Username: `vagrant`  
        Password: `vagrant`  

#### Acknowledgements :  
 -  Deploys Base Vagrant Box : Ubuntu 14.04 Desktop: [box-cutter/boxes/ubuntu1404-desktop] (https://vagrantcloud.com/box-cutter/boxes/ubuntu1404-desktop)  
 -  Uses the [vagrant-reload] (https://github.com/aidanns/vagrant-reload) plugin by [Aidan] (https://github.com/aidanns)  
 -  Uses the Eclipse [project-import] (https://github.com/seeq12/eclipse-import-projects-plugin) plugin by [Seeq] (https://github.com/seeq12)  
 -  Commands for installing Java 8 have been taken from <a href="https://github.com/aglover">Andrew Glover's<a> <a href="https://github.com/aglover/ubuntu-equip">github repository</a>.
 -  Commands for installing Eclipse have been taken from <a href="http://blog.versioneye.com/2015/05/05/setting-up-a-dev-environment-with-vagrant/">this blog</a>.
