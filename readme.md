1. https://mattermost.emse.fr/m-info-2020/channels/security

https://ecampus.emse.fr/course/view.php?id=258 

https://ecampus.emse.fr/course/index.php?categoryid=70

2. ![blaster worm propagation](https://github.com/anindameister/security/blob/master/snaps/2.PNG)
3. ![blaster worm propagation hand written](https://github.com/anindameister/security/blob/master/snaps/3.jpeg)
4. paper https://github.com/anindameister/security/blob/master/IEEE_Security_Privacy_Blaster_Final.pdf

# should have been done in labtainers

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

# class on 22 September, 2020

- contains the part where ram memory mgmt has been explained  https://drive.google.com/file/d/1bhuGlI2fChvbgJ7yLhfiiieu7tAA1sCb/view?usp=sharing

- disponsible- available
- backup is not present in the same location as the data
- In computer security, a DMZ or demilitarized zone (sometimes referred to as a perimeter network or screened subnet) 
is a physical or logical subnetwork that contains and exposes an organization's external-facing services 
to an untrusted, usually larger, network such as the Internet.
- Spoofing is an impersonation of a user, device or client on the Internet. 
It's often used during a cyberattack to disguise the source of attack traffic. 
The most common forms of spoofing are: DNS server spoofing – Modifies a DNS server in order to redirect a domain name to a different IP address.
- http: 80(protocol)/43(dns) port
- WAF(web applocation firewall): to check the situation of http connection: could be the encryption, header of http protocol containing info: - info transporting data: data could be bad data in terms of containing bug
- vpn gives low level network access to school via httpm protocol
- An intrusion detection system (IDS) is a device, or software application that monitors a network or systems for malicious activity or policy violations.

![Saas,PAA,IAAS](https://github.com/anindameister/security/blob/master/snaps/26.PNG)

- Transport Layer Security (TLS) is the successor protocol to SSL. TLS is an improved version of SSL. 
It works in much the same way as the SSL, using encryption to protect the transfer of data and information.

- SSL Stands for secure sockets layer. Protocol for web browsers and servers that allows for the authentication, encryption and decryption of data sent over the Internet. 
Wildcard SSL certificates Type of certificate used to secure multiple subdomains.

# working in labtainers

#### cat /etc/passwd

![cat /etc/passwd](https://github.com/anindameister/security/blob/master/snaps/27.PNG)

- courtesy : https://www.youtube.com/watch?v=TbJ-yQhB4WE

- c signifies char file
- d directory file
- simple - signifies that it's an ordinary file
- 1. rw : read/write/but no execution(super user with admin privilges)
- 2. other permissions of the group users
- 3. other users
- 4. no of links in the file, here, 1 so no other association to other directory
- 5. name of owner
- 6. name of the group
- 7. size of the file in bytes
- 8. dob of file creation
- 9. name of the file

![cat /etc/passwd](https://github.com/anindameister/security/blob/master/snaps/28.PNG)

- checking inside the file
- one line stores info of one user

![cat /etc/passwd](https://github.com/anindameister/security/blob/master/snaps/29.PNG)

- different fields come into existence by the use of : in the line

![cat /etc/passwd](https://github.com/anindameister/security/blob/master/snaps/30.PNG)

- 1. user name- should be between 1 to 32 characters in length
- 2. password: x character indictes encrypted password is stored in etc/shadow file
- 3. user id: each user must be assigned a userID. userID=0 is assigned for root user and 1to99 are reserved for other pre-defined accounts
further 100-999 is assigned for administrative and system accounts or groups
- 4. GroupID or GID, which is stored in etc/groupFile
- 5. the user id information, comment screen, info about user
- 6. home directory, the absolute path where the user would log in. if directory doesn't exist then the user's directory is the main or the root directory
- 7. command of shell, the absolute path of the command of shell bin/bash


# Buffer Overflow Attack - Computerphile

- https://www.youtube.com/watch?v=1S0aBV-Waeo&feature=youtu.be
- A Buffer Overflow exploit is a situation where we're using a low level function like C to write a string into a piece of memory which is only of certain length.
- but we're trying to write on that memory, something, which is longer than that; and it then overwites the later memory address which in turn can cause a lot of problems.
- 1st thing on talk, roughly what happens to memory when a program is run. in this regards, we're talking about c program in linux but this can be extended to work on many different languages and operating systems
- when a program is run on an OS, at that time we're making to run that program with some shell and we type in the command like theFileName.extensionOfTheProgrq,
- now, at that time, the OS would effectively call, as a function, the main method of your code
- but your actual process, your executable, will be held in a memory in a very specific way, and it's consistent between different processes

![big block of Ram](https://github.com/anindameister/security/blob/master/snaps/31.PNG)

- we have a big block of Ram, we dont know how big our RAM is because it is varied, but we use called Virtual Memory Translation to say that, everything in here, this is 0x000000... which i sthe bottom of the memory
- and up at the top we have 0xfffff which is the equivalent of 11111memory addresses, all the way upto 32 or 64bit and it starts from 0.

![memory addressses](https://github.com/anindameister/security/blob/master/snaps/32.PNG)

###### 32bit ram

- https://techterms.com/help/difference_between_32-bit_and_64-bit_systems#:~:text=One%20bit%20in%20the%20register,temporary%20values%20besides%20memory%20addresses.
- https://stackoverflow.com/questions/21197010/how-long-is-a-memory-address-typically-in-bits
- https://web.stanford.edu/class/cs101/bits-bytes.html

- 32-bit and 64-bit are commonly used to describe processor architecture or design. 
- A 32-bit processor includes a 32-bit register, which can store 2^32 or 4,294,967,296 values. 
- A 64-bit processor includes a 64-bit register, which can store 2^64 or 18,446,744,073,709,551,616 values. 
- Therefore, a 64-bit register is not twice as large as a 32-bit register, but is 4,294,967,296 times larger. 
- That's a big difference, but how does it affect computing performance?
- The CPU register stores memory addresses, which is how the processor accesses data from RAM. 
- The processor uses 32 bits to store an address.
- With 32 bits, you can store 2^32 distinct numbers, ranging from 0 to 2^32 - 1. 
- "Byte addressing" means that each byte in memory is individually addressable, i.e. there is an address x which points to that specific byte. 
- Since there are 2^32 different numbers you can put into a 32-bit address, we can address up to 2^32 bytes, or 4 GB.
- Conclusion: 32 bits means 2^32 memory address is accessible in one cycle. Each memory address points to 1 byte of data. So 2^32 memory address is 4Gigabytes of data
- Similarly 64bits CPU can address 2^64=(16 exabytes)18,446,744,073,709,551,616 bytes, or 17,179,869,184 gigabytes (16 exabytes) of memory.
![memory addressses](https://github.com/anindameister/security/blob/master/snaps/33.PNG)

#### Buffer Overflow Attack - Computerphile contd...

- now, when we use the ram memory, there are already certain areas of this memory that are always allocated to certain things
- so up at the top, we have the kernel things, so; this will be commandline parameters that we can pass to our program and environment variables and so on

![kernel intro](https://github.com/anindameister/security/blob/master/snaps/34.PNG)

- down at the bottom, we have something called text. That's the actual code of our program. The machine instructions that we compiled, get loaded in there. 

![text](https://github.com/anindameister/security/blob/master/snaps/35.PNG)

- And that's the read only, because we dont want to be messing about that, down there

![data](https://github.com/anindameister/security/blob/master/snaps/36.PNG)

- just on the top of text, we have data. So in data, uninitialised and initialised variables get held here in data.
- And then we have the heap. Now, the heap may have been mentioned from time to time, it's where you allocate large things in your memory.

![heap](https://github.com/anindameister/security/blob/master/snaps/37.PNG)

- Big area of memory that you can allocate huge chunks on to do various things and what you do with that is, of course, upto your programme.
- And then up there, we have something which is perhaps the most important bit, in someway anyway, is the stack.

![stack](https://github.com/anindameister/security/blob/master/snaps/38.PNG)

- Now, the stack holds the local variables of your functions and when you call a new function like, like printf followed by some parameters; that gets put on the end of the stack.
- So, the heap grows in the upward direction towards the stack,as you add memory in ways of allocating large things, and the stack grows towards the heap

![stack&heapGROWTH](https://github.com/anindameister/security/blob/master/snaps/39.PNG)

#### stack

- let's focus on stack, because that's where a lot of these buffer overflows happen.
- we can also have overflows in other areas, but stack is the important part

![stack, high and low memory addresses](https://github.com/anindameister/security/blob/master/snaps/40.PNG)

- the stack grows downwards from high memory addresses to low memory addresses. So, when we add something onto the end of the stack it gets put on and move towards low memory address point

![stack, high to low memory addresses](https://github.com/anindameister/security/blob/master/snaps/41.PNG)

- some very acurate and fine details about stack is given below
https://www.tutorialspoint.com/data_structures_algorithms/stack_algorithm.htm
- there's a very minimal difference between arraylist and linkedlist
https://www.tutorialspoint.com/differences-between-arraylist-and-linkedlist-in-java#:~:text=LinkedList%20uses%20Doubly%20Linked%20List%20to%20store%20its%20elements.&text=ArrayList%20is%20slow%20as%20array,not%20much%20bit%20shifting%20required.&text=ArrayList%20implements%20only%20List.

#### stack from the video contd..

- let's consider that we have some programme that's calling a function.
- A function is some area code that does something and then returns back to where it was before.

![using the calling function](https://github.com/anindameister/security/blob/master/snaps/42.PNG)

- when the calling function wants to make sure of something, it adds its parameters that it's passing onto the stack 

![using the calling function](https://github.com/anindameister/security/blob/master/snaps/43.PNG)

- so the parameter A and B are added onto the stack in reverse order

![parameter A and B are added onto the stack in reverse order](https://github.com/anindameister/security/blob/master/snaps/44.PNG)

![parameter are added onto the stack in reverse order](https://github.com/anindameister/security/blob/master/snaps/45.PNG)

- And then the assembler code for this function will make something called a "call" and that would jump to somehwere else in the memory and work with these two things and it's the nature of this stack that causes us to have problems

![assembly language](https://github.com/anindameister/security/blob/master/snaps/46.PNG)

- let's look into some code and find out how it works

```
#include <stdio.h>
#include <string.h>

int main(int argc, char** argv)
{
	char buffer[500];
	strcpy(buffer, argv[1]);
	return 0;
}

```

- the above C code allocates some memory on the stack and then copies a string into it from the command line

- so in the C programme, we got the main function that takes the number of parameters given and a pointer to those variables that you've got 

- pointers below
https://www.javatpoint.com/c-pointers#:~:text=The%20pointer%20in%20C%20language,function%2C%20or%20any%20other%20pointer.&text=int*%20p%20%3D%20%26n%3B%20%2F%2F,variable%20n%20of%20type%20integer.
- %d decimal output, %x hexadecimal output
- pointer program, a general one , which is easier to understand is below
![pointer programme example](https://github.com/anindameister/security/blob/master/snaps/47.PNG)

#### stack, c program, pointer, video dude contd..

- and they'll be help in the kernel area of our memory
- we have allocated a buffer that's 500 character long and then we call a function called strcpy, which will copy our commandline parameter into argv into our buffer

![buffer,strcpy](https://github.com/anindameister/security/blob/master/snaps/48.PNG)


- our function puts on a return address which is replacing the code we need to go back to once we've done strcpy

![return](https://github.com/anindameister/security/blob/master/snaps/49.PNG)

- so that's how main knows where to go after it's finished
- And then we have put on a reference to the base pointer in our previous function. It's not important to this video.

![basePointer](https://github.com/anindameister/security/blob/master/snaps/50.PNG)
- this is just going to be our EBP base pointer

- the below is our allocated space for buffer and it's 500 long

![our allocated space for buffer](https://github.com/anindameister/security/blob/master/snaps/51.PNG)

![our allocated space for buffer](https://github.com/anindameister/security/blob/master/snaps/52.PNG)

- if we write into it something that's longer than 500, we're going to to straight past the buffer,over this(EBP base pointer), and crucially over our return variable

- And that's where we point back to something we shouldn't be doing (Kali Linux Distribution)

- we have a small function in the c program, that does our copy from the commandline. So compilation, done, and now running it with "Hello"
- this will copy "hello" into this buffer and then simply return, so nothing happens.

- putting the commandline parameter Hello while running the program
![putting the commandline parameter Hello while running the program](https://github.com/anindameister/security/blob/master/snaps/53.PNG)

###### basic programme
- we can consider another program that can copy "Hello" into the buffer and process it; example make it all upper-case.
- so we can get a function which makes it all, uppercase
- so I can copy hello off, and then can change this newcopy to be all uppercase, and then you output it in the screen
- and that doesn't even have to be main and it could be just any function

##### GDB:- basic Linux commandline debugger
- GDB not adviseable unless you really like seeing lots of Assembly and doing really low-level Linux things
- so we go to the location and do GDB, this initiates GDB
- type in 
```
list
```
- and it shows the code for our function. So we can see that it just compiled our function
- done from our computer
![done from our computer](https://github.com/anindameister/security/blob/master/snaps/89.PNG)


![programme from gdb](https://github.com/anindameister/security/blob/master/snaps/54.PNG)
- now, it knows this because the compiler included this information along with the executable
- we can also show the machine code for this so we can say "disas main"(in the gdb) disassemble main and we can see the code for main
![disas main](https://github.com/anindameister/security/blob/master/snaps/55.PNG)
- the above snap shows the actual cpu instructions that will be run
- check Steve Bagley's video for Assembly
- however, a couple of very important things are:
- the line here sub of 0x1f4 from %esp, that's allocating 500 for the buffer
![0x1f4 from %esp](https://github.com/anindameister/security/blob/master/snaps/56.PNG)
- we're at the begining of the stack and from there we go 500 in the below direction and that's where our buffer goes
###### starting from stack and going 500 units to buffer
![starting from stack and going 500 units to buffer](https://github.com/anindameister/security/blob/master/snaps/57.PNG)
- so the buffer sitting to the left of the image but is lower on memory than the rest of our variables

- now, we can run this program from GDB and if it crashes then we can look at the registers and find out what's happened
- we start like this, run Hello , so GDB starts the program and says Hello and it exited normally
![GDB starts the program and says Hello](https://github.com/anindameister/security/blob/master/snaps/58.PNG)
- now, we can pass something a little bit longer than Hello
- If we pass something that's over 500, then this buffer will go over this base pointer and this return value, and break the code
![method to go over the EDB and break the code](https://github.com/anindameister/security/blob/master/snaps/59.PNG)
- It should just crash it. Python, for example, can produce strings based on simple scripts on the command line
- we say, run and then pass it with Python script of print....41(that's the "a" character), let's say 506 times
- python script to print the "a" character, 506 times
![python script to print the "a" character, 506 times](https://github.com/anindameister/security/blob/master/snaps/60.PNG)
- just a little bit more than 500 so that it is going to cause somewhat of a problem but not a catastrophe and then we run that, so it has received a segmentation fault
![segmentation fault](https://github.com/anindameister/security/blob/master/snaps/61.PNG)

- now the segmentation fault is something, what a Cpu will send back to you when you're trying to access something in memory you shouldn't be doing.
###### stack situation at threshold which is 500
![stack situation at threshold which is 500](https://github.com/anindameister/security/blob/master/snaps/62.PNG)
###### stack situation at crossover of the threshold which is 500 and reaching 506
![stack situation](https://github.com/anindameister/security/blob/master/snaps/63.PNG)
- Again the segmentation fault is something, what a Cpu will send back to you when you're trying to access something in memory you shouldn't be doing.
- But that's not what has actually happened because we overwrote somewhere we shouldn't, what happening is that the return address was half over written with these 41s
###### stack situation where return address was half overwritten by 41s as shown in the photo
![stack situation where return address was half overwritten by 41s as shown in the photo](https://github.com/anindameister/security/blob/master/snaps/64.PNG)
- so is doesn't know what it is
- so there's nothing in memory at 0xb7004141, and if there is, it doesn't belong to this process. It's not allowed, so it gets segmentation fault
- so if we now, change that to 508("a" character number of times), we're going 2 bytes further along, which means we're now overwriting the entirety of our return address.
!["a" character number of times is 508](https://github.com/anindameister/security/blob/master/snaps/65.PNG)
!["a" character number of times is 508 and overwriting the entirety of our return address](https://github.com/anindameister/security/blob/master/snaps/66.PNG)
- so we're overwriting the "return address" with 41s. Now, if there were some virus code at 414141, that's a big problem. 
- so we run this and now can see that the return address is now 0x414141
![return address is now 0x414141](https://github.com/anindameister/security/blob/master/snaps/67.PNG)
###### the register situation
![the register situation](https://github.com/anindameister/security/blob/master/snaps/68.PNG)
- we can now see that in the register, the instruction/construction pointer is now trying to point ot 0x414141 which means that it has read this return value and tried to return to that place in the code and run it, and ofcourse it can'take

#### code broken, now what do we do

- what we need to do is change this return value to somewhere where we've got some payload we're trying to give- we're trying to produce
- let's quit the debugger and checkout the payload
- this payload is a simple, very short programme in Assembler, that puts some variables on the stack and then executes the system call to tell it to run a shell- to run a new command line
- our shell code, would depend on linux OS and not on the CPU type 
![our shell code](https://github.com/anindameister/security/blob/master/snaps/69.PNG)
- this is just a string of different commands. Crucially, this xcd\x80 is throwing a system interrupt, which means that it's going to run the system call.
###### system interrupt
![system interrupt](https://github.com/anindameister/security/blob/master/snaps/73.PNG)
###### system call
![system call](https://github.com/anindameister/security/blob/master/snaps/74.PNG)

- what this will actually do is run something called ZSH, which is an old shell that doesn't have a lot of protections involved
###### zsh
![ZSH](https://github.com/anindameister/security/blob/master/snaps/70.PNG)
###### shell scripting
![shell scripting](https://github.com/anindameister/security/blob/master/snaps/71.PNG)

###### contd....
- let's go back to our debugger , gdb, and we're gonna run again but this time, a slightly more malicious code
- \x41 * 508 and then putting our shell code
![shell scripting](https://github.com/anindameister/security/blob/master/snaps/75.PNG)
![shell scripting](https://github.com/anindameister/security/blob/master/snaps/76.PNG)
- to craft an exploit from this, what we need to do is remember the fact that strcopy is going to copy into our buffer.
- so we're gonna start at the beginning of buffer which is the point not facing base pointer
![start at the beginning of buffer](https://github.com/anindameister/security/blob/master/snaps/77.PNG)

- so we're gonna start at the beginning of the buffer. we want to overwrite the memory of the return address with somewhere pointing to our malicius code
- now, we can't necessarily know for sure where our malicious code might be stored elsewhere on the disk, so we dont worry about that or memory
- so we want to put it in this buffer. so we're going to put some maliciouscode in here and then we're going to have a return address that points back into it
- Memory moves around slightly. When you run these programmes, things change slightly, environment variables are added or removed, things move around
- so, we want to try and hedge our bets and get the rough area that this will go in
###### No-Op sled
![start at the beginning of buffer, No-Op sled](https://github.com/anindameister/security/blob/master/snaps/78.PNG)
![No-Op sled](https://github.com/anindameister/security/blob/master/snaps/79.PNG)
###### machine instruction for "just move to the next one"
![No-Op sled](https://github.com/anindameister/security/blob/master/snaps/80.PNG)
- anywhere we land in that No-Op is going to tick along to out malicious code
- so we have a load of \x90s , then we have our shell code. That's our malicious payload that runs our shell
- return address, right in the right place, that points back right smack in the middle of these \x90s
![No-Op sled](https://github.com/anindameister/security/blob/master/snaps/81.PNG)
- and what that means is, even if it moves a bit, it'll still work
- just like having a slope almost
![No-Op sled](https://github.com/anindameister/security/blob/master/snaps/82.PNG)
#### 2bcontd....


# gdb lesson

- labtainer gdblesson
![labtainer gdblesson](https://github.com/anindameister/security/blob/master/snaps/83.PNG)
- Alternatively, you can write the C program through the Terminal in gedit as follows:

$ gedit sampleProgram.c
- compiled
$ gcc [programName].c -o programName
- run
$ ./programName

# shell

- https://www.youtube.com/watch?time_continue=8&v=9y5TCwVU8iE&feature=emb_logo

- kernel is the nucleus of a computer
- kernel makes the communication happen between the software and hardware, possible
- kernel is the innermost part of the OS, and the shell is a part of outermost part of the OS
- a shell in Linux OS, takes input from user in the form of commands, processes them and gives the output
- shell is an interface through which a user works on the program's commands and scripts

![shell](https://github.com/anindameister/security/blob/master/snaps/91.PNG)

-  a shell is accessed by a terminal which runs it
- when you're in the terminal the shell issues a command prompt which is usually the dollar sign, where in you can type your input, which is then executed when you enter the enter key.
-  So if we press PWD then the output is displayed in the terminal
- the shell wraps around the delicate interior of an OS, protecting it from accidental damage, hence the name shell
- there are two main shells in Linux, the first one in Bourne shell
- the prompt for the Bourne shell is the dollar sign and it's derivative is the POSIX shell, also known as sh. Korn shell is also known as sh and Bourne Again Shell also known as bash which is the most popular of them all
- The second one, which is another important shell in Linux is "The C" shell. The prompts for this shell is "%" and it's sub-categories are "C shell" aka csh, "Tops C SHell" aka tcsh

#### what is shell scripting and it's uses

- writing a series of command for the shell to execute is called shell scripting
- it can combine the lengthy and repetative sequence of commands into a single and simple script which can be stored and executed anytime
- this reduces the efforts required by the end-user

#### steps to create a shell-script

1. create a file with vi editor or any other text eidtor
2. name the script file with extension .sh
3. start the script with 
```
#! /bin/sh
```
4. write some code
5. save the script file as filename.sh
6. for executing the script type
```
bash filename.sh
```
- here  #! called shebang which directs the script to the interpretator location
- creating a small script with VI editor"
```
vi samplescript.sh
```
- pressing "I" key in the keyboard, we enter the Insert mode in the editor
- enter the command
```
#!/bin/sh
ls
```
- esc to get out of insert mode
- :wq and enter
- running the command and checking the output
![shellOutput](https://github.com/anindameister/security/blob/master/snaps/92.PNG)

#### adding shell comments

- #comment

#### shell variables

![shell variables](https://github.com/anindameister/security/blob/master/snaps/93.PNG)
- read command
![read command](https://github.com/anindameister/security/blob/master/snaps/95.PNG)
- using the read command
![using the read command](https://github.com/anindameister/security/blob/master/snaps/96.PNG)


![shell variables' usage and seeing the output](https://github.com/anindameister/security/blob/master/snaps/94.PNG)

#### summary shell
- CLI- command line interface
![summary](https://github.com/anindameister/security/blob/master/snaps/97.PNG)
![summary](https://github.com/anindameister/security/blob/master/snaps/98.PNG)
![summary](https://github.com/anindameister/security/blob/master/snaps/99.PNG)


# x86 Assembly crash course

- https://www.youtube.com/watch?v=75gBFiFtAb8&feature=youtu.be

#### binary exploitation
- process of taking compiled executables and making them do, what you want them to do.
- to understand binary exploitation, we need to first understand what binary is and how it works on level, before exploiting it
- hitting the compile option after running the c code, leads to generation of a text file with a special extension; which is read by a compiler which would inturn convert the code that have been written in form of C into a series of executable operations
- each operation compires of sequence of bytes called the operation code, or opcode
- reading opcodes, which the computer would be executing is almost impossible. Aseembly comes in here, which translates the language of the computer to human readable
- let's understand the basic elemements of an executable before getting into assembly
- every C program has 4 main components, heap,stack,registers, instructions
- at this time, there are mainly 2 main architectures that dictates how a program is compiled and executed; 32 and 64bit
- let's go over the 32 bit architecture and 32 bit assembly
- heap in the memory is designed for the purpose of manual memory allocation
- we just need to know for now, because heap is complicated; that whenever functions such as malloc and calloc are called as well as global or static variables are declared.
- registers are essentially small storage areas in your processor. They can be used to store memory addresses and values or anything that can be represented by 8 bytes or less
- in the x86 architecture, there are 6 general purpose registers: eax, ebx, ecx, edx,esi,editing
- the above registers are generally used in as-needed basis
- there are also 3 registers for specific purposes: ebp, esp, eip
###### the stack
- the stack is data-structure comprised of elements that are added or removed with 2 operations(Push,POP)
- push adds element on top of the stack
- and pop removes element from the top of the stack
- each element on the stack is assigned to stack address, elements that are higher on the stack has a lower address. In other words, the stack grows towards lower memory addresses
![stack address](https://github.com/anindameister/security/blob/master/snaps/103.PNG)
- whenever a function is called, that function is setup with what is called a stack frame
- all the local variables of that function would be stored in that functions' stack frame
![stack frame](https://github.com/anindameister/security/blob/master/snaps/104.PNG)
- ebp register, also known as base pointer register, comes into action. This ebp register contains the address of the base of the current stack frame
- esp, stack pointer, contains the address of the top element of the current stack frame
- all the space between these two registers, make up the  current stack frame of whatever function is currently being called.
- all the stack addresses outside the current stack frame is considered to be junk by the compiler
###### the C program
![the C program](https://github.com/anindameister/security/blob/master/snaps/105.PNG)
- first the value of the argument is pushed on to the stack, then the return address of the function is pushed on to the stack
- the return address is simply the 4bytes address of the instruction that'll be executed, as soon as the function is gone out of scope
- then the base pointer is pushed on to the stack
- then the stack pointer is given the value of the base pointer as seen below
![base and stack pointers' intro](https://github.com/anindameister/security/blob/master/snaps/106.PNG)
- finally the stack pointer is decremented to make room for the local variables
- depending on your compiler, the number of bytes that the stack pointer is decremented by , may vary
- all of the space b/w stack and the base pointer, makes our stack frame
- this sequence of instruction is called the function prolog
- the prolog is performed whenever a function is called
- since our function's 1st local variable is 0, so th evalue 0 will be moved into the memory address which is 4 bytes below the base pointer; and that's because an integer is 4bytes
- just a reminder, the value of the argument which is pushed initially on to the stack is at the highest memory address
- now the local variable is at location ebp-4("-" is used because it is moving to the lower memory address)
- again, the value of our argument is located 8bytes above the base pointer, which is not in the function stack frame
- again, the function stack frame is b/w ebp and esp
- since we have created a local variable, which is initialised with a value equal to the value of argument, hence the argument which is not residing yet into the function stack frame needds to be brought intot the function stack frame
- there's a catch here, the values on the stack cannot be moved directly to another location on the stack
- this is where our general purpose registers come in
- the value of the argument to our function must be first copied into one of our general purpose registers, then the value is moved into the memory address 4bytes below our first variable(term "below" because we're going towards lower memory address") and 8bytes below the base pointer
- now, both of our local variables have been initialised and can bbe accessed for later use
![base and stack pointers' and return address existing below ebp intro](https://github.com/anindameister/security/blob/master/snaps/107.PNG)

# assembly
- two syntaxes assembly is usually written is:- at&t and intel. the instruction presentation is different here and we'll go for intel way of represntation
- instruction format
- if we wanna copy the value of the arg2 into the location of arg1
![instruction format](https://github.com/anindameister/security/blob/master/snaps/108.PNG)
- mov in general
![mov in general](https://github.com/anindameister/security/blob/master/snaps/109.PNG)
- if we wanna move a value located in the stack into the eax register and let's say that the stack variable is located at ebp-0x8
```
mov eax,ebp-0x8
```
then the above would copy the address of ebp-0x8 because that's basically the address on the stack or where our variable is located and not the value
in order to copy the value, or where ebp-0x8 is pointing to , we got to do,
```
mov eax,[ebp-0x8]
```
introduce the square brackets(think of it as deference operator in C)
- add 
![add](https://github.com/anindameister/security/blob/master/snaps/110.PNG)
- final value of eax is 15
-sub
![sub](https://github.com/anindameister/security/blob/master/snaps/111.PNG)
- push
- decrements the esp location, move it to lower address
![push](https://github.com/anindameister/security/blob/master/snaps/112.PNG)
- pop
- takes register as argument
- it moves the top element of the stack into the register specified by it's argument and then increment the stack pointer, thereby popping off the top element from the stack
![pop](https://github.com/anindameister/security/blob/master/snaps/113.PNG)
![pop](https://github.com/anindameister/security/blob/master/snaps/114.PNG)
- lea(load effective address)
- it places the adress specified by it's 2nd operand into the register specified by it's first operand
- this is mainly used to obtain a pointer into memory region
#### loops and if statements would come together to determine the order in which the instructions are executed
###### eip register aka instruction pointer
![eip](https://github.com/anindameister/security/blob/master/snaps/115.PNG)
###### compare
- similar to sub
- except like sub where it stores the instruction in the first arg1
- it would set a flag in the processor where it store values which are 0,<0,>0
![compare](https://github.com/anindameister/security/blob/master/snaps/116.PNG)
- compare instruction is always followed by jump instruction 
- je(jump equal to, ne-not equal, g:greater than)
![jump](https://github.com/anindameister/security/blob/master/snaps/117.PNG)
```
compare 1,3
jump  if less than
```
- in the above scenario, jump would be taken
- greater than, comes to picture instead of less than; then jump would not be taken and the eip would just move to the next instruction like below

![jump](https://github.com/anindameister/security/blob/master/snaps/118.PNG)
###### call
- call instruction calls a function whether it is a user-defined or plt(printf or scanf)function.
- this instruction takes one argument and is equivalent to push eip, jump argument
- in order words, it'd push the return address of the function being called on to the stack and then move eip onto the first instruction of the function 
![call](https://github.com/anindameister/security/blob/master/snaps/119.PNG)
###### leave
- the leave instruction is called at the end of every function
- it eseentially destroys the current stack frame by setting the stack pointer to the base pointer and popping the base pointer off the top of the stack
![leave](https://github.com/anindameister/security/blob/master/snaps/120.PNG)
![leave](https://github.com/anindameister/security/blob/master/snaps/121.PNG)

###### return
- the return instruction alwaays follow the leave instruction
- since the base pointer has already been popped off the stack, the return address of the function is now at the top of the stack
- the return instruction would pop the return address off the top of the stack and then set the instruction pointer to that address
![return](https://github.com/anindameister/security/blob/master/snaps/122.PNG)
![return](https://github.com/anindameister/security/blob/master/snaps/123.PNG)


# cryptography [[1]](#1).

![cryptography](https://github.com/anindameister/security/blob/master/snaps/126.PNG)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/127.PNG)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/127.jpeg)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/128.PNG)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/129.PNG)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/130.PNG)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/131.PNG)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/132.PNG)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/133.jpeg)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/134.jpeg)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/135.jpeg)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/136jpeg)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/137.jpeg)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/133.PNG) [[3]](#3). 

- types of cryptography

![cryptography](https://github.com/anindameister/security/blob/master/snaps/134.PNG)

![cryptography](https://github.com/anindameister/security/blob/master/snaps/135.PNG) 

![cryptography](https://github.com/anindameister/security/blob/master/snaps/136.PNG) 

![cryptography](https://github.com/anindameister/security/blob/master/snaps/137.PNG) 

- symmetric cryptography 

![cryptography](https://github.com/anindameister/security/blob/master/snaps/138.PNG) 
 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/139.PNG) 

# South Indian Dude  

- video 1- network security basic concept [[4]](#4).

![cryptography](https://github.com/anindameister/security/blob/master/snaps/140.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/141.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/142.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/143.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/144.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/145.PNG) 

- NETWORK SECURITY - TYPES OF ATTACKS video2 [[5]](#5).


![cryptography](https://github.com/anindameister/security/blob/master/snaps/1146.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/1147.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/1148.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/1149.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/1150.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/1151.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/1152.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/1153.PNG) 

- NETWORK SECURITY - SECURITY SERVICES video 3 [[6]](#6). 

![cryptography](https://github.com/anindameister/security/blob/master/snaps/148.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/149.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/150.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/151.PNG) 

- NETWORK SECURITY - SUBSTITUTION TECHNIQUES video4 [[7]](#7). 

![cryptography](https://github.com/anindameister/security/blob/master/snaps/205.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/206.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/207.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/208.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/209.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/210.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/211.PNG) 

- NETWORK SECURITY - TRANSPOSITION TECHNIQUES video5 [[8]](#8). 

![cryptography](https://github.com/anindameister/security/blob/master/snaps/220.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/221.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/222.PNG) 
![cryptography](https://github.com/anindameister/security/blob/master/snaps/223.PNG) 

- NETWORK SECURITY - FEISTEL STRUCTURE video6 [[9]](#9). 

![cryptography](https://github.com/anindameister/security/blob/master/snaps/230.PNG) 

- block cipher design principle
1. block size: the size of plain text would be equal to that of th4e cipher text

- the tick marks are used for increasing the security. Eg: increasing the number of rounds, increases the security

![cryptography](https://github.com/anindameister/security/blob/master/snaps/231.PNG) 


- NETWORK SECURITY- AES (ADVANCED ENCRYPTION STANDARD) Algorithm

![cryptography](https://github.com/anindameister/security/blob/master/snaps/250.PNG) 

![cryptography](https://github.com/anindameister/security/blob/master/snaps/251.PNG) 

![cryptography](https://github.com/anindameister/security/blob/master/snaps/252.PNG) 

###### block diagram

![cryptography](https://github.com/anindameister/security/blob/master/snaps/253.PNG) 

![cryptography](https://github.com/anindameister/security/blob/master/snaps/254.PNG) 

# iptables [[10]](#10). 

- powerful linux tool
- it is used to create quick and powerful firewall for your system
- it provides an interface to work with packet filtering framework of linux kernel called netfilter

![iptables](https://github.com/anindameister/security/blob/master/snaps/1154.PNG)

- in simple terms, it's a powerful tool to manage network packets, coming to and going out of your system
- so with iptables you can block, access or take other actions with network traffics based on different user defined conditions

![iptables](https://github.com/anindameister/security/blob/master/snaps/1155.PNG)

- 3 important terms: tables, chains, rules
- 5 tables, 3 are main and each has different roles
#### tables
- 1. filter table: main table, which is also default meaning that when nothing is mentioned in regards to table the rule will apply for filter table

![iptables,filter table](https://github.com/anindameister/security/blob/master/snaps/1156.PNG)

- as the name suggests the role of this table is of filter packets that's making decision whether to let a packet continue tot he intended destination or to deny it's request
- this is the table which provides majority of functions of iptables
- 2. NAT table

![iptables,NAT table](https://github.com/anindameister/security/blob/master/snaps/1157.PNG)

- as the name suggests, it is used to provide network address translation rules. The rule of this table would determine whether to modify or how to modify the packet source or destination addresses in order to route the packet in NAT setup where direct access is not possible

- 3. Mangle table

![iptables,NAT table](https://github.com/anindameister/security/blob/master/snaps/1158.PNG)

- this table is used to alter the ip headers of the packet
- eg: of the alteration of ip headers, we can adjust (TTL)time to live of the packet; either lengthening or shortening the valid network hops that the packet can sustain

- 4. RAw table

![iptables,NAT table](https://github.com/anindameister/security/blob/master/snaps/1159.PNG)

- the raw table is used for connection tracking
- it provides a mechanism for marking packets, to view packets as a part of ongoing connections or session

- 5. security table

- the security table is used to set internal SELinux, security context marks on packets which will affect how SELinux or other system that can interpret SELinux security context handle these packets

#### chains

- chains are the routes or points to packet where you can apply rules
- there are 5 chains in iptables
- prerouting, input,forward,output, post routing

![iptables,chains](https://github.com/anindameister/security/blob/master/snaps/1160.PNG

- all chains are not available for all tables.
- each chain gives you option to take action on the packet and that particular point in the packet route.

- 1. prerouting chain is applied to any incoming packet very soon after entering the network stack

![iptables,prerouting chain](https://github.com/anindameister/security/blob/master/snaps/1161.PNG)

- this chain is processed before any routing decision have been made regarding where to send the packet

- 2.  input chain is a point, post prerouting, when packet enters a system

![iptables,prerouting chain](https://github.com/anindameister/security/blob/master/snaps/1162.PNG)

- 3. forward chain is applied to a packet that is forwarded through your system
- 4. output chain is applied to a packet originated from your system and going out
- 5. post-routing is oppsoite of pre-routing, this is applied to outgoing or forwarded traffic after routing decision has taken place and just before packet has been put on the wire

![iptables,chain](https://github.com/anindameister/security/blob/master/snaps/1163.PNG)

- now all chains are not available for all tables
- so we got to know which chain available for which table
- we should also know the order in which chain is called for each table and also chain traversal order

![iptables,order of chain](https://github.com/anindameister/security/blob/master/snaps/1164.PNG)

- the above figure shows the order in which chain is called for different table and also the avilability of chain for each table
- so for filter table according to the figure, we have three chains i.e. input, forward and output

#### chain traversal order

![iptables,chain traversal order](https://github.com/anindameister/security/blob/master/snaps/1165.PNG)

- chain traversal order which is actually the path, how packet traverses
- so for incoming packets to the local system , the traversal order is pre-routing and then input
- the rest is according to the above snap

#### iptable rules

![iptables,rules](https://github.com/anindameister/security/blob/master/snaps/1166.PNG)

- as each chain is called, the packet will be checked against each rule within the chain, in order
- if the packet, doesn't match then the next rule in the chain is examined
- if it does match then, the next rule is specified by the value of the target
- now each rule has two component: matching component and target component.

![iptables,rules](https://github.com/anindameister/security/blob/master/snaps/1167.PNG)

- macthing component is differnt conditions available to define rules

![iptables,rules](https://github.com/anindameister/security/blob/master/snaps/1168.PNG)

- so we can match by protocol type, destination or source address, destination or source port, input or output interface, headers etc..
- these can be combined to create really complex rule sets

- next is the target component 
- the target componet is the action that's triggered when a packet meets the matching criteria of a rule
- now there are two types of target, terminating and non-terminating target

![iptables,rules](https://github.com/anindameister/security/blob/master/snaps/1169.PNG)


- terminating target is the actions which end the further traversal in that particular chain. Eg: accept.drop,queue, reject, return, or mved to any user-defined chain

- non-terminating target, you perform an action and then continue evaluation within the chain

![iptables,rules](https://github.com/anindameister/security/blob/master/snaps/1170.PNG)


- note: not all action is available for every chain and table, hence the table and chain types dictates the action available

![iptables,rules](https://github.com/anindameister/security/blob/master/snaps/1171.PNG)

# wireshark

- wireshark is a tool to check what is going on in a network. Eg: seeing passwords and other info, on a network
- wireshark is a graphical interface
- tshark is the corresponding commandline interface
- npcap or winpcap to capture live network data. This is used by Wireshark.
- usbpcap is used to capture usbtraffic
- npcap lookback dapter gets installed in windows with wireshark installation. this nocap loopback can be found in network connection.

#### within wireshark [[11]](#11).

- EIGRP is a routing protocol
- OSPF is another routing protocol
- there'll be a lot of traffic in the network connected to windows, but we'll just filter to only see certain traffic types, in our case telnet
- so we'll do a telnet to a device in our network

# Intrusion Detection and Prevention Systems (IDS/ IPS) | Security Basics [[12]](#12).

- IDS detects
- IPS prevents
- more details in slide, very basic in the video. 

#### IDS bypassing 
- video 1 for 3Nov,2020; slide 39

# What is SIEM? Security Information & Event Management Explained [[13]](#13).

# Encryption of communications 

#### IPSEC 
- micronuggets, no technical term has been used as per slide [[15]](#15).
- technical terms used but requires patience to understand [[14]](#14).

![IPSEC](https://github.com/anindameister/security/blob/master/snaps/155.PNG)

- SSL is a cryptographic protocol that uses explicit connections to establish secure communication between web server and client. 
- TLS is also a cryptographic protocol that provides secure communication between web server and client via implicit connections. 
- It's the successor of SSL protocol.

# ssh [[16]](#16).

#### SSL, TLS, HTTP, HTTPS Explained [[17]](#17).










## References
<a id="1">[1]</a> 
https://www.khanacademy.org/computing/computer-science/cryptography/ciphers/a/shift-cipher


<a id="2">[2]</a> 
https://www.geeksforgeeks.org/vigenere-cipher/

<a id="3">[3]</a> 
https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher

<a id="4">[4]</a> 
https://www.youtube.com/watch?v=VJelZrYc49c&list=PLLOxZwkBK52Ch0y2lLtfepy4Lt_SVkwo3&index=1

<a id="5">[5]</a> 
https://www.youtube.com/watch?v=_zq4qTc9Jmg&list=PLLOxZwkBK52Ch0y2lLtfepy4Lt_SVkwo3&index=2

<a id="6">[6]</a> 
https://www.youtube.com/watch?v=oUUmAQLea-A&list=PLLOxZwkBK52Ch0y2lLtfepy4Lt_SVkwo3&index=3

<a id="7">[7]</a> 
https://www.youtube.com/watch?v=L2NAQbZeRXo&list=PLLOxZwkBK52Ch0y2lLtfepy4Lt_SVkwo3&index=4

<a id="8">[8]</a> 
https://www.youtube.com/watch?v=eKMmrDy3LCQ&list=PLLOxZwkBK52Ch0y2lLtfepy4Lt_SVkwo3&index=5

<a id="9">[9]</a> 
https://www.youtube.com/watch?v=drI2shandyk&list=PLLOxZwkBK52Ch0y2lLtfepy4Lt_SVkwo3&index=6

<a id="10">[10]</a> 
https://www.youtube.com/watch?v=vbhr4csDeI4&t=13s

<a id="11">[11]</a> 
https://www.youtube.com/watch?v=4_7A8Ikp5Cc

<a id="12">[12]</a> 
https://www.youtube.com/watch?v=rvKQtRklwQ4

<a id="13">[13]</a> 
https://www.youtube.com/watch?v=GbFtSDnPZBQ

<a id="14">[14]</a> 
https://www.youtube.com/watch?v=tuDVWQOG0C0

<a id="15">[15]</a> 
https://www.youtube.com/watch?v=CuxyZiSCSfc

<a id="16">[16]</a> 
https://www.youtube.com/watch?v=qWKK_PNHnnA

<a id="17">[17]</a> 
youtube.com/watch?v=hExRDVZHhig


































































