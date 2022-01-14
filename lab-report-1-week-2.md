# Lab Report 1

## Installing VScode
To download the code editor for this class use this link: [DOWNLOAD](https://code.visualstudio.com/)  


![vscode download](https://user-images.githubusercontent.com/97620200/149451131-ebc4dc7c-8de0-4f50-b225-6d875dac440d.jpg)

Once the application is open, it will look like this, and we can now create new files or open existing ones.  
  

![vscode open](https://user-images.githubusercontent.com/97620200/149451427-65845644-fb69-4e7a-a422-5d862243bed0.jpg)

## Remotely Connecting
To remotely connect we have to first install OpenSSH

Go into your computer **Settings > Apps > Apps & Features > Add a feature**

Now you should install OpenSSH Client and OpenSSH Server

Using this [link](https://sdacs.ucsd.edu/~icc/index.php) lookup the course specific account tied to your student username and ID

With VSCode open, we need to open a new terminal

![new terminal](https://user-images.githubusercontent.com/97620200/149453422-2b2f1315-d565-47d6-913d-7ede1d0bf234.png)

Your account for CSE 15l, taken Winter of 2022, will look like cs15lwi22xxx

with your own unique combination of letters to replace xxx

To connect to the ieng6 server at UCSD, we need to type the following code

```
ssh cs15lwi22xxx@ieng6.ucsd.edu
```
If you are then prompted to enter a password, this should be the password for your UCSD account, which will be veiled as you type

## Trying Some Commands
Now that your personal device is remotely connected to a UCSD server we can try basic commands

`cd` stands for "change directory"

Typing in `cd ~` will take you back to the home or default directory

Typing in `ls` will "list" the files found within the current directory


![remote](https://user-images.githubusercontent.com/97620200/149455882-25b968ce-f457-49e7-a36e-f0738850f953.jpg)

Typing `exit` will return you to your own computer

## Moving Files with `scp`

If we create a new file named `heyThere.java` with the contents
```
class heyThere {
    public static void main(String[] args){
        System.out.println("Hey! Hello! Hi there!");
    }
}
```

Into the command line, from the directory in which you saved your file, again replacing xxx,

type `scp heyThere.java cse15lwi22xxx@ieng6.ucsd.edu:~/`

Now, using `ls` we will see the new file

![scp](https://user-images.githubusercontent.com/97620200/149457421-e9e3c596-fccd-4f43-81bb-9a3cd285e058.jpg)

## Setting an SSH Key

In the terminal on your computer

Type `ssh-keygen` to generate an SSH Key

In this case, we want to remove the need to type in our account password each time

When the terminal prints `Enter file in which to save the key (/Users/Rachel/.ssh/id_rsa):` press the enter key

Likewise press the enter key in response to `Enter passphrase (empty for no passphrase):`

and again when we see `Enter same passphrase again:`



