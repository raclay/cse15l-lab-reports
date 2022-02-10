Rachel Claypool
# Lab Report 3: Streamlining ssh Configuration


## ssh Configuration
![config](https://user-images.githubusercontent.com/97620200/153480443-ba11bff8-f5e2-403f-afe0-3a9a26e3f8b3.jpg)
Inside `C:\Users\Rachel\.ssh` I added a file called config.  Even though it only contains text, it is important that this file is saved as type File and not Text Document.  I used Notepad to edit and paste the given text into this file.  The characters following "Host:" will be your alias.  


## Logging in
![ssh](https://user-images.githubusercontent.com/97620200/153480491-b78d50db-98d9-4a97-9698-7085c1eb0bd9.jpg)
Now, all I need to do is type into the command line `ssh ieng6` and I can connect remotely to the server.  If I wanted to change this alias to anything of my choosing, I would be able to inside that config file.  

--------
If I still was having a difficult time remembering ieng6, and wanted my alias to be "abcd", I would replace ieng6 with abcd in the config file and type `ssh abcd` into the command line instead.
![new config](https://user-images.githubusercontent.com/97620200/153483324-a8ae257e-1e87-4beb-b3d0-45d081da6f28.jpg)
![new ssh](https://user-images.githubusercontent.com/97620200/153483755-716c5c8e-a183-4e30-835a-4aeccec081dc.jpg)



## Using the scp command
![newfile](https://user-images.githubusercontent.com/97620200/153480510-b7e7abee-4a3b-44b5-af43-c7f2d963105b.jpg)
I changed my alias back to ieng6, so when I want to copy a file from my personal laptop to my account, I need only type `scp newFile.java ieng6:~/`.  I need to be in the directory on my laptop containing newFile.java and I will successfully find my new file in my remote account.
