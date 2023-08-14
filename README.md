# Home_lab-1
# This is my home lab where I exploit Metasploitable 2 a vulnerable machine using Parrot OS made by SourceForge.

In this step i'm going to add this account to sudoers to execute command as root
![Screenshot 2023-08-13 195424](https://github.com/ARG1509/Home_lab-1/assets/115385507/189dc0a5-609d-443f-bf9b-2fc1e48e2c00)

I'm going to add myhomelab account under "# User privilige specification" as "myhomelab ALL=(ALL:ALL) ALL" after typing it i hit CTRL + X and ENTER to save and exit.
![Screenshot 2023-08-13 195641](https://github.com/ARG1509/Home_lab-1/assets/115385507/7ca0044a-3506-4dd8-96a1-3d75f0102c0d)

Then do a "sudo apt update" command to update the permissions.
![Screenshot 2023-08-13 195935](https://github.com/ARG1509/Home_lab-1/assets/115385507/663142b1-436e-4d76-a35e-2da7554a24e0)

Now i can deploy the Metasploitable 2 machine and log in using "msfadmin" for both user and password.
![Screenshot 2023-08-13 200429](https://github.com/ARG1509/Home_lab-1/assets/115385507/73362f24-772f-4d66-8995-cc653b42bd71)

After login in i run the "ifconfig" command to gather some information about the machine such as the IP address 
![Screenshot 2023-08-13 201911](https://github.com/ARG1509/Home_lab-1/assets/115385507/286542eb-97ae-4a4b-9a68-e480bc649ac2)

Then i deploy my parrot OS machine and run a simple nmap command to get some information.
![Screenshot 2023-08-13 202318](https://github.com/ARG1509/Home_lab-1/assets/115385507/43da7dbc-d4c5-4b76-9213-43ac8a0c99e4)

After running the nmap command i see that there's a lot of open ports that's because this machine was designed to be vulnerable and for this lab i'm going access the machine using the telnet service located on port 23
![Screenshot 2023-08-13 202554](https://github.com/ARG1509/Home_lab-1/assets/115385507/c44d18e2-dc21-4d56-b017-f06d0314a773)

I did some research about the telnet service and found out i can connect to the vulnerable machine using telnet.
![Screenshot 2023-08-13 215846](https://github.com/ARG1509/Home_lab-1/assets/115385507/7a35f3d6-795d-4fa1-b8ea-bb36d124f5ca)

then i make sure i have telnet installed on my machine by using the "sudo apt install telnet" command
![Screenshot 2023-08-13 202900](https://github.com/ARG1509/Home_lab-1/assets/115385507/23cd6881-e1a8-4458-92b8-3533704f1a12)

After installing telnet we can run the telnet command followed by the IP address and port (23) of the vulnerable machine 
![Screenshot 2023-08-13 203121](https://github.com/ARG1509/Home_lab-1/assets/115385507/cf182988-288b-45d3-bbc7-1c0f8b52f24b)

Then i successfuly accessed the machine using telnet and ran the same "ifconfig" command i did the first time.
![Screenshot 2023-08-13 203234](https://github.com/ARG1509/Home_lab-1/assets/115385507/4b47e639-ceff-4f70-a11f-5be5df213376)
