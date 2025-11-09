# Small-IT-Environment
To practice in an IT environment, we will be doing the following with our Virtual machines. On how to simulate an office Network, Users, and Groups administration, set up, secure, and troubleshoot file sharing. 

## Tools / Resources:

- VirtualBox: To create and run Virtual Machines
- Windows 10 ISO: Your Windows workstation
- Ubuntu Desktop ISO: Your Linux Workstation
- Network Configuration: Allows your VMs to talk to each other
- Command Line tools: To check IPs and test connections
- File Sharing Tools: To connect Linux to Windows folders

## Command Used: 
- sudo apt update && sudo apt upgrade -y ( This will update all system packages)
- Ip addr (check ip address)
- Ping : connects with other networks

- Sudo addgroup
- Sudo adduser
- Sudo usermod -aG  (name of group) (name of user)

## Windowas: 
ipconfig ( Checks IP Address)

## ALWAYS CHECK FOR UPTADES 
To do this on Ubuntu we first need to update it using  

- sudo apt update && sudo apt upgrade -y

This updates all the packages as well.

<img width="1912" height="1025" alt="updating ubuntu" src="https://github.com/user-attachments/assets/58ce7754-c118-44e8-9253-1f5ecfd7ac3c" />


## SIMULATING AND INTERNAL OFFICE NETWORK
For this, we are using two virtual machines, the first one is Windows 10, and the other VM is Ubuntu. To start this off, we are going to check the IP address information for Windows 10, the one we are going to use is the IPv4 address; therefore, we are going to use 10.0.2.15. Now, to connect from my other VM, I would have to use the IP address I was able to locate. Now, to connect to Windows, I would use the ping <ipaddress>  command on Ubuntu. If you are connected, you will see the following saying that there is a connection between both machines.

<img width="1899" height="986" alt="Connection between VMs " src="https://github.com/user-attachments/assets/f6d87cc4-c035-46d1-91ab-01f437504e92" />


## HOW TO CREATE USERS / GROUPS AND ADD THEM TO GROUPS.
The Way I Will Show The Process Is First Talk About It, And Then Showa a Picture Of The Steps For The Visual Learners, And So It Goes With The Material.

## Windows 
Creating a user and then adding them to a group consists of one simple step to start this it would be searching Computer Management in the Windows search bar. GO to the local users and group tab as you can see on the left side of the window and then click on the user folder inside. Right click and click on the new user. Now we are going to create a user. On the User name, we are going to input techsupport, name, and password. If you want to have one, I did put one in and click OK. As you can see, the new user has been added to the group. I underlined it in red to show you that it was created.

<img width="912" height="995" alt="opening computer management" src="https://github.com/user-attachments/assets/a3d4a2b8-a26d-4ceb-99b4-11faf5a4e489" />

<img width="934" height="991" alt="creating a user 1" src="https://github.com/user-attachments/assets/df2c827c-1149-4a8b-8ee8-5beb4b212b48" />

<img width="948" height="1015" alt="creating a user 2 (right click to create" src="https://github.com/user-attachments/assets/94cab59e-c1be-4519-a721-9c439a932958" />

<img width="933" height="1011" alt="user created 3" src="https://github.com/user-attachments/assets/0661f96e-c11c-4a54-a204-c95ce00fd86e" />

<img width="938" height="1024" alt="user creater on user folder" src="https://github.com/user-attachments/assets/1b3e1b20-4641-48ab-81bc-a88c57440c82" />

##

Now for creating a group is basically the same thing; we just need to click in the folder that says group in the same tab that says local users and group. Right click in the window, click the new group, and you get yourself in the Create New User tab. We are going to name it ITDept and add techsupport users to this group. To do this, we are going to click on the add button for members. After you are in, go to the bottom text box and text tech support, and click on the one that showed up for you. Then click ok, then ok one more time, and there you have a new group as well as a member added to the group.

<img width="944" height="1013" alt="creating new group 1" src="https://github.com/user-attachments/assets/626f269e-ea99-479a-8b3c-264633fdd148" />

<img width="924" height="998" alt="creating group 2" src="https://github.com/user-attachments/assets/06b154eb-5558-4576-a3f3-2987a2a2638a" />

<img width="925" height="1011" alt="checking user is added" src="https://github.com/user-attachments/assets/eb573761-4b82-483f-a717-48b5006d694a" />


## Linux
Creating a user and new group in a linux environment it's a bit more straightforward. We are going to search for the terminal once we are going to use the following command. But remember its cap sensitivity so everything needs to be the same.

- Sudo addgroup itdept

- Sudo adduser techsuport

When you are in the command for adding a new user, you will be asked to enter Full name, Room Number, Work and Home phone, and other. For this, I just entered techsupport for full name, room 1, and a fake number, and left the rest empty. When you have done that, we are going to confirm that the information that we entered is correct by entering Y. Now the following command will allow us to add the new user to the group itdept.

- Sudo usermod -aG itdept techsupport

<img width="971" height="989" alt="creating user and adding to group on ubuntu " src="https://github.com/user-attachments/assets/cb38ce5a-c76e-486a-aeb9-40bcdf481613" />














