1. https://mattermost.emse.fr/m-info-2020/channels/security
2. ![blaster worm propagation](https://github.com/anindameister/security/blob/master/snaps/2.PNG)
3. ![blaster worm propagation hand written](https://github.com/anindameister/security/blob/master/snaps/3.jpeg)
4. paper https://github.com/anindameister/security/blob/master/IEEE_Security_Privacy_Blaster_Final.pdf
5. unix commands

- pwd : (present working directory) to see what your home directory is 

![pwd](https://github.com/anindameister/security/blob/master/snaps/3.PNG)

- ls : List the contents of your home directory by using the ls (list) command:

![ls](https://github.com/anindameister/security/blob/master/snaps/4.PNG)

- we started with a folder which had another folder named security, so basically the smart enough unix system ignores the empty part
- point to be noted, that the hiden git folder is not showed up

- ls –a
- the above even lists the hidden files and in our case it is git folder

![ls -a](https://github.com/anindameister/security/blob/master/snaps/5.PNG)

- ls –al: Get a bigger picture of the contents of the current directory (such as owner and size) by also using the -l (long) option 

![ls -al](https://github.com/anindameister/security/blob/master/snaps/6.PNG)

![ls -l](https://github.com/anindameister/security/blob/master/snaps/7.PNG)

- ls -al: shows the bigger picture including that of the hidden files
- ls -l: shows the bigger picture EXCLUDING that of the hidden files
- ll: shows the bigger picture EXCLUDING that of the hidden files and it is the shorter version of ls -l

- ls recording/ 
1. now this shows the contents of the recording folder
2. please note that while we did an ls to check the contents of the directory, recording/ came up and that's how I got to know that "recording/" is the one we got to get into
3. let's take a moment to check the hassle below

![ls -l](https://github.com/anindameister/security/blob/master/snaps/8.PNG)

4. windows: dir == linux: ls; windows: cd == linux: cd; windows:cd.. ==linux cd ..(note the space)

- mkdir folderName=linux and the same in windows to create a folder
- to create a file in linux: touch fileName.txt whereas in windows type nul > filename.txt
- again remeber this type nul > your_file.txt
- the url for the above: https://stackoverflow.com/questions/30011267/windows-equivalent-of-touch-i-e-the-node-js-way-to-create-an-index-html

5. ll -a : to list all the contents with details

6. let's take a moment to check the hassle below

![ll -a](https://github.com/anindameister/security/blob/master/snaps/9.PNG)

7. - renaming a file
 mv someUnixCommandsList.txt renaming2something.txt

![mv](https://github.com/anindameister/security/blob/master/snaps/10.PNG)

- renaming a folder

![renaming a folder](https://github.com/anindameister/security/blob/master/snaps/11.PNG)

- moving a folder
- renaming happends if the folder doesn't exist
- if the folder exists then folder move happens
- format: nameOfTheFolder2bRenamedORmoved name2bMOVEDintoOR2brenamedBY

![moving a folder](https://github.com/anindameister/security/blob/master/snaps/12.PNG)

8. copying(cp) a file 2 a folder
- cp nix-commands.pdf unixcommands/

![copying(cp)](https://github.com/anindameister/security/blob/master/snaps/13.PNG)

- copying(cp) a hidden file to another folder

![copying(cp)](https://github.com/anindameister/security/blob/master/snaps/200.PNG)

- '/' can also be removed in case of a file copy to a folder

![copying(cp)in case of a file copy to a folder](https://github.com/anindameister/security/blob/master/snaps/14.PNG)

- copying a folder to another folder

source: https://devconnected.com/how-to-copy-directory-on-linux/#:~:text=In%20order%20to%20copy%20a,destination%20directories%20to%20be%20copied.&text=As%20an%20example%2C%20let's%20say,folder%20named%20%E2%80%9C%2Fetc_backup%E2%80%9D.

![website](https://github.com/anindameister/security/blob/master/snaps/17.PNG)

- cp -r classnotes unixcommands

![copying(cp)in case of a folder copy to another folder](https://github.com/anindameister/security/blob/master/snaps/15.PNG)

- the above can be exactly applied for hidden folders as well

- cp -r .git unixcommands

![copying(cp)in case of a hidden folder copy to another folder](https://github.com/anindameister/security/blob/master/snaps/16.PNG)

- You can, of course, rename the file while copying. Copy the hidden file again,renaming it in the process:
- from hidden to hidden status: cp -r .git testingFolder/.gitRenamed
- from hidden to non-hidden status:  cp -r .git testingFolder/gitRenamed

![copying(cp) and renaming](https://github.com/anindameister/security/blob/master/snaps/18.PNG)

- copying a hidden file to another folder and renaming in the process

![copying(cp) and renaming](https://github.com/anindameister/security/blob/master/snaps/201.PNG)

9. removing

![removing from staging area](https://github.com/anindameister/security/blob/master/snaps/19.PNG)

- removing a file
- rm newfile

- removing a folder
- rmdir  creatingadirectoryjust2bremoved

![removing](https://github.com/anindameister/security/blob/master/snaps/20.PNG)

- removing a folder containing stuffs

- rm -r newfoler2

![removing](https://github.com/anindameister/security/blob/master/snaps/21.PNG)

- got to check for windows(check the link below for windows)

- https://www.windows-commandline.com/delete-directory-from-command-line/

- admin rights to delete folder https://www.thewindowsclub.com/youll-need-provide-administrator-permission-delete-folder

#### What Causes the You do not have Permission to View this Object’s Security Properties Error?

- Some other program or service is using your file or folder simultaneously, preventing you from editing its permission settings. If this is the case, a simple restart should be more than enough to solve the problem.

- Removing contd..

- rm -r newfoler2 is in regards to delete the complete folder including the contents

- rm newfile is in regards to getting into a folder and removing the particular file

- rm newfolder/.hidden*  is in regards to staying outside the folder named newfolder and deleting all the contents whose name starts with .hidden

- rm newfolder/new*  is in regards to staying outside the folder named newfolder and deleting all the contents whose name starts with new

![removing all](https://github.com/anindameister/security/blob/master/snaps/22.PNG)

10. displaying the contents of a particular file: cat (concatenate) command

- url for all cat commands : https://www.geeksforgeeks.org/cat-command-in-linux-with-examples/

![displaying the contents of a particular file](https://github.com/anindameister/security/blob/master/snaps/24.PNG)

- cat particularFile.txt  :make sure to give the extension or else it wouldn't work

![displaying the contents of a particular file](https://github.com/anindameister/security/blob/master/snaps/23.PNG)

11. Display text on the screen by using the echo command:
- echo "hello world"

![echo command](https://github.com/anindameister/security/blob/master/snaps/25.PNG)















