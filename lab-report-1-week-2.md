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

To connect to the ieng6 server at UCSD, we need to type the following code

```
ssh cs15lwi22xxx@ieng6.ucsd.edu
```
