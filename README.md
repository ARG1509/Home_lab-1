# Home_lab-1
# This is my home lab where I exploit Metasploitable 2 a vulnerable machine using Parrot OS made by SourceForge.

In this step I'm going to add this account to sudoers to execute commands as root
[Screenshot 2023-08-13 195559](https://github.com/ARG1509/Home_lab-1/assets/115385507/2a2a6fe6-5a31-4668-a108-8471129a6dfe)



I'm going to add myhomelab account under "# User privilege specification" as "myhomelab ALL=(ALL:ALL) ALL" after typing it I use CTRL + X and ENTER to save and exit.
![Screenshot 2023-08-13 195641](https://github.com/ARG1509/Home_lab-1/assets/115385507/b00cceab-36a7-4d86-8caa-ae76cab14c7f)



Then do a "sudo apt update" command to update the permissions.
![Screenshot 2023-08-13 195935](https://github.com/ARG1509/Home_lab-1/assets/115385507/cba8288f-f448-4f6f-9be4-9f789eb368fc)



Now I can deploy the Metasploitable 2 machine and log in using "msfadmin" for both user and password.
![Screenshot 2023-08-13 200429](https://github.com/ARG1509/Home_lab-1/assets/115385507/22035d6a-27bb-49f8-aa51-ec5b44752480)


After login in I run the "ifconfig" command to gather some information about the machine such as the IP address.
![Screenshot 2023-08-13 201911](https://github.com/ARG1509/Home_lab-1/assets/115385507/eba103b5-eba2-41f4-9f5a-4663ed113606)


Then I deploy my parrot OS machine and run a simple nmap command to get some information.
![Screenshot 2023-08-13 202318](https://github.com/ARG1509/Home_lab-1/assets/115385507/e49fb395-7038-4029-b644-ce1c1373f665)


After running the nmap command I see that there's a lot of open ports that's because this machine was designed to be vulnerable and for this lab I'm going to access the machine using the telnet service located on port 23
![Screenshot 2023-08-13 202554](https://github.com/ARG1509/Home_lab-1/assets/115385507/6da9c624-d810-419e-8979-5fa86f4444e9)


I did some research about the telnet service and found out I can connect to the vulnerable machine using telnet.
![Screenshot 2023-08-13 215846](https://github.com/ARG1509/Home_lab-1/assets/115385507/1c0c1e1e-a76d-4a57-8039-8b8a5582cd71)


then I make sure I have telnet installed on my machine by using the "sudo apt install telnet" command
![Screenshot 2023-08-13 202900](https://github.com/ARG1509/Home_lab-1/assets/115385507/031e9810-6b48-4ccf-abf5-017b0f125c46)


After installing telnet we can run the telnet command followed by the IP address and port (23) of the vulnerable machine 
![Screenshot 2023-08-13 203121](https://github.com/ARG1509/Home_lab-1/assets/115385507/9c7471e9-0b8a-450b-a5f5-88eb7621789d)


Then I successfully accessed the machine using telnet and ran the same "ifconfig" command I did the first time.
![Screenshot 2023-08-13 203234](https://github.com/ARG1509/Home_lab-1/assets/115385507/eb096252-3e2b-4c65-8dc0-e4e0688711f7)

