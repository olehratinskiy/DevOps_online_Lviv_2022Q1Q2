## PART 1. HYPERVISORS

#### What are the most popular hypervisors for infrastructure virtualization?
- Oracle VirtualBox
- Microsoft Hyper-V
- VMware ESXi/vSphere
- Xen / Citrix XenServer

#### Briefly describe the main differences of the most popular hypervisors.
There are two types of hypervisors. The first type runs directly on the host's hardware. Another runs in a window as a typical computer application.
<br/><br/>
## PART 2. WORK WITH VIRTUALBOX

### First run VirtualBox and Virtual Machine

**Created a virtual machine VM1_Ubuntu_Ratinskiy and made a clone of it called VM2_Ubuntu_Ratinskiy**
![img_15.png](img/img_15.png)
<br/><br/>
**Created a group of these two VMs**
![img_16.png](img/img_16.png)
![img_17.png](img/img_17.png)
<br/><br/>
**Formed a branched tree of snapshots for VM1_Ubuntu_Ratinskiy**
![img_18.png](img/img_18.png)
<br/><br/>
**Exported VM1_Ubuntu_Ratinskiy as a file and imported it again**
![img_19.png](img/img_19.png)
![img_20.png](img/img_20.png)
![img_21.png](img/img_21.png)
<br/><br/>

### Configuration of virtual machines

**Configured a USB connection to the VM**
![img.png](img/img_24.png)
![img.png](img/img_25.png)
<br/><br/>
**Created a shared folder between VM1 and the host**
![img.png](img/img_22.png)
![img.png](img/img_23.png)
<br/><br/>
**Made a table of possible connections (between VM1, VM2, Host, Internet) using different network modes**
| Mode        | VM to Host | Host to VM   | VM1 to VM2   | VM to Net/LAN | Net/LAN to VM |
| ----------- | -----------| -------------| -------------| --------------| --------------|
| Host-only   | Yes        | Yes          | Yes          | No            | No            |
| Internal    | No         | No           | Yes          | No            | No            |
| Bridged     | Yes        | Yes          | Yes          | Yes           | Yes           |
| NAT         | Yes        | Port forward | No           | Yes           | Port forward  |
| NAT Network | Yes        | Port forward | Yes          | Yes           | Port forward  |
<br/><br/>

### Work with CLI through VBoxManage

VBoxManage list
![img.png](img/img.png)
<br/><br/>
VBoxManage showvminfo
![img_1.png](img/img_1.png)
<br/><br/>
VBoxManage startvm
![img_2.png](img/img_2.png)
<br/><br/>
VBoxManage createvm
![img_3.png](img/img_3.png)
<br/><br/>
VBoxManage modifyvm
![img_4.png](img/img_4.png)
<br/><br/>
VBoxManage clonevm
![img_5.png](img/img_5.png)
<br/><br/>
VBoxManage snapshot
![img_6.png](img/img_6.png)
<br/><br/>
VBoxManage controlvm
![img_7.png](img/img_7.png)
<br/><br/>

## PART 3. WORK WITH VAGRANT

vagrant init hashicorp/precise64
vagrant up
![img_8.png](img/img_8.png)
![img_9.png](img/img_9.png)
<br/><br/>
mobaxterm date
![img_11.png](img/img_11.png)
<br/><br/>
vagrant ssh-config
vagrant halt
vagrant destroy
![img_10.png](img/img_10.png)
<br/><br/>
create Vagrant box
![img_13.png](img/img_13.png)
![img_14.png](img/img_14.png)
<br/><br/>
My Vagrant box:
[test_box](https://app.vagrantup.com/olehratinskiy/boxes/test_box)