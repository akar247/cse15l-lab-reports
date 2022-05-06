# CSE-15L-LAB-REPORT3-week6 -- Aman Kar

## 5/8/2022


[Home Page](index.md)

<br>

### All Group Choice Options (1-3)

<br>

### 1. Streamlining ssh Configuration
<br>

#### a. Edit and config file, edited with VS Code

![Image](configIn-ssh.png)
<br>

![Image](configEdit.png)

<br>

The pictures above illustrates hwo to find the config file in the hidden ssh directory as well as the edit to make on the config file. For the `User` portion, make use of the [UCSD Account lookup](https://sdacs.ucsd.edu/cgi-bin/alloc-query) to find your user specific username.

<br>
<br>

#### b. Logging with `ssh` command

![Image](sshLogin.png)

<br>

Utilizing the command `ssh ieng6`, the terminal automatically my key to log in with the associated username in the config file. As seen in the picture, with that command, the terminal logged me into the `ieng6` server. 


#### c. `scp` command to copy files

![Image](copyFile.png)

<br>

As seen in the image above, utilizing the comand `scp <file> cs15lsp22@ieng6.ucsd.edu:~/` I was able to copy a file from my local server to the ieng6 server. With the `ls` command, I can see the file in my ieng6 server. 



<br>
<br>

### 2. Setup Github Access from ieng6

<br>

#### a. Public key on Github Server
![Image](gitSshKey.png)

<br>
As seen in the above picture, the SSH key is stored on my personal account of the the online Github server. 

<br>

#### b. Private key on user account
![Image](idRsaLocation.png)
![Image](privateKeyIeng6.png)

<br>
As seen in the picture above, the id_rsa private key is stored in my .ssh file. Obviously I cannot show the contents of the file since that would allow anyone to login to my account. I also included an image of creating the key on my user account on ieng6 server. This allows me to use push and commit on the ieng6 server.

<br>

#### c. Running Git `commit` & `push`

![Image](gitCommandsIeng6.png)

<br>

To test running `commit` and `push` git commands on the ieng6 server, I will be using the addition of this text as the change to commit and push to the GitHub server. As seen in the picture above, the commands `add` , `commit`, and `push` worked correctly. This can be seen in the change of `git status` before and after pushing the changes. More evidence of this push is the link to the [commit](https://github.com/akar247/cse15l-lab-reports/commit/daf68d948e68d463a2bea4463ab38d5d868e41ed).


