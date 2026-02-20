# LockdownGuest

Lockdown Guest Ubuntu Account

By default, ubuntu comes with a guest account, so, I’m going to disable access to this account by locking it down so it cannot be used. All this will be done from the root account ($)
 
<img width="239" height="247" alt="Image" src="https://github.com/user-attachments/assets/a93b12ce-81dd-4da3-a975-db56ab2c5a08" />

To get started I’m in the root account which is indicated on the terminal with the sign $. The command cd etc/lightdm/ put me in the lightdm file thus the command cd means change directory. From there I listed what’s in that file with the command ls.
 <img width="473" height="88" alt="Image" src="https://github.com/user-attachments/assets/92100a2f-42b8-4361-8ac1-3461fd14fca7" />

In this file there are 3 other files which are lightdm.conf lightdm.conf.d and user.conf. The lightdm folder contains settings which involve logins, so I edited this file by using the vi which is the visual editor. I used the command sudo vi lightdm.conf because that is the file I want to edit. With the file opened I scrolled down to the bottom of the file then pressed o which put my cursor into an edit mode, then I typed in allow-guest=false. What this does it deny access into the guest account.  

<img width="561" height="221" alt="Image" src="https://github.com/user-attachments/assets/a80a2e61-dd45-4674-bbb5-c9b7fe0bfedc" />

In order for the changes to take place I had to restart the system, to restart the system I typed the command sudo reboot then put my password, upon entry to the root account the guest account is no more there to be logged into.
 
<img width="337" height="275" alt="Image" src="https://github.com/user-attachments/assets/6722ea66-c76d-43e6-97d9-f0d87f36edcf" />
