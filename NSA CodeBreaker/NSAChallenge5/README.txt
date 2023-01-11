5: Was not completed, hoping for partial credit

Used pwnbdg on the ssh-agent binary with the provided core file. 
To find the location of the string for the server name, started with “/tmp”. 
Searched for variables around that location for the address of the idlist table data type. 
We know the idlist address will be around the address for the server’s name as its close in proximity 
in the original ssh-agent code which is open source. Found at open source code for ssh-agent at 
https://github.com/openssh/openssh-portable/blob/master/ssh-agent.c . After that I loaded in the pytype 
struct for idtable so that pwn gdb can follow the trail of symbol names to the key values we want. There was 
only one entry in the table. I dumped its shielded prekey into one file and its shielded private value into 
another. For the next steps I found this website that covers it and followed it.
 
https://security.humanativaspa.it/openssh-ssh-agent-shielded-private-key-extraction-x86_64-linux/

Essentially I downloaded a copy of the open ssh directory and set it up.  Then followed the commands they 
did in gdb on ssh-keygen file which took the 2 found variables and generated the key needed to decrypt the 
file. This is where I ran out of time and stopped. I tried continuing it later bc I thought I just needed to 
do very little however I ran into some problem using the key to decrypt it. If I had more time after 
understanding this lab to the level I do now I’m sure I could have finished it.
