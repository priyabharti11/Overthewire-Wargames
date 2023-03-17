# Overthewire-Wargames

Overthewire Wargames is a platform for prcaticing Linux Concepts in the form of fun filled games.

<h1>Level 0</h1>
<p> 
<h2> Level Goal</h2>
   <h4> The goal of this level is for you to log into the game using SSH. The host to which you need to connect is <br>
        bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged <br>
        in, go to the Level 1 page to find out how to beat Level 1. 
   </h4>
</p>
        
  <h2>Commands you may need to solve this level</h2>

  <h4> SSH : <br>
   
   SSH, also known as Secure Shell or Secure Socket Shell, is a network protocol that gives users,particularly system   administrators, a secure way to access a computer over an unsecured network.

   SSH also refers to the suite of utilities that implement the SSH protocol. Secure Shell provides strong password
   authentication and public key authentication, as well as encrypted data communications between two computers         connecting over an open network, such as the internet.
</h4> 

   <h2> Solution</h2>
   
   <h3> Step 1:</h3>
   
   Install Openssh client and server programs in your linux system through terminal
   
   
   <h3>
    Command :</h3>
    
       sudo apt install openssh-client
       sudo apt install openssh-server
   <br>
   
   <h3> Step 2:</h3>
  
   Enable the and start the ssh service in your system.
   
   
   <h3>
    Command :</h3>
    
      sudo systemctl enable ssh
   <br>
   
   <h3> Step 3:</h3>
   
   Now Connect to the Overwire Lab using ssh using the hostname and password given.
   
   
   <h3>
    Command :</h3>
    
       ssh bandit0@bandit.labs.overthewire.org -p 2220
       
      (I used '-p' to specify the port 2220 becasue i got an error that my system was using port 22 )
    
   </h3>
   <br>
   <br>
   <br>
   <br>
   <br>
   <br>
   <br>
   <br>
   
<h1>Level 1</h1>
<p> 
<h2> Level Goal</h2> 
<h4> 
   The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH.  Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.
</h4>
</p>

 <h2> Solution</h2>
   
   <h3> Step 1:</h3>
   
   Read and copy the password from the 'readme' file in home directory of bandit0 user.
   
   
<h3>
    Command :
</h3>
    
       cat readme
       
      ( Used cat because 'readme' is not a directory its a file so we need to read it , we cant used cd command )
      ( A password will appear, copy it using 'Ctrl+Shift+C' command )
 <br>
 
 
<h3> Step 2:</h3>
 
  Now just type exit to exit the current 'bandit0' user.
 
 
 <h3>
    Command :
</h3>
    
       exit
<br>
       

<h3> Step 3:</h3>

   Now you need to again use ssh to access the 'bandit1' user.
 
<h3>
    Command :
</h3>
    
       ssh bandit1@bandit.labs.overthewire.org -p 2220
       
      ( I used '-p' to specify the port 2220 becasue i got an error that my system was using port 22 )
      ( use password which u copied from readme file )
 <br>
  <br>
   <br>
   <br>
   <br>
   <br>
   <br>
   <br>
   <br>
 

 
 
 <h1>Level 2</h1>
<p> 
<h2> Level Goal</h2> 
<h4> 
   The password for the next level is stored in a file called - located in the home directory.
</h4>

<h3>NOTE : Use "cat ./-" or "cat < -" to see what is in the "-" file.</h3>
</p>

 <h2> Solution</h2>
   
   <h3> Step 1:</h3>
   <h4> 
      Read and copy the password from the '-' file in home directory of bandit1 user.
   </h4>
   
<h3>
    Command :
</h3>
    
       cat ./-
   
      ( A password will appear, copy it using 'Ctrl+Shift+C' command )
 <br>
 
 
<h3> Step 2:</h3>

  Now just type exit to exit the current 'bandit1' user.
 
 
 <h3>
    Command :
</h3>
    
       exit
<br>
       

<h3> Step 3:</h3>
<h4> 
     Now you need to again use ssh to access the 'bandit2' user.
 </h4>
<h3>
    Command :
</h3>
    
       ssh bandit2@bandit.labs.overthewire.org -p 2220
       
      ( I used '-p' to specify the port 2220 becasue i got an error that my system was using port 22 )
      ( use password which u copied from '-' dashed file )
 <br>
 <br>
 <br>
 <br>
 <br>
 <br>
 <br>
 <br>
 <br>
 <br>
 
 
 
 
 
 <h1>Level 3</h1>
<p> 
<h2> Level Goal</h2> 
<h4> 
   
</h4>

<h3>NOTE : Use cat "file name with multiple words" to see what is in the file. Enclose the file name under double quotes which have a long name with spaces.</h3>
</p>

 <h2> Solution</h2>
   
   <h3> Step 1:</h3>
   <h4> 
      Read and copy the password from the 'spaces in the filename' file in home directory of bandit2 user.
   </h4>
   
<h3>
    Command :
</h3>
    
       cat "spaces in the filename"
   
      ( A password will appear, copy it using 'Ctrl+Shift+C' command )
 <br>
 
 
<h3> Step 2:</h3>

  Now just type exit to exit the current 'bandit1' user.
 
 
 <h3>
    Command :
</h3>
    
       exit
<br>
       

<h3> Step 3:</h3>
<h4> 
     Now you need to again use ssh to access the 'bandit3' user.
 </h4>
<h3>
    Command :
</h3>
    
       ssh bandit3@bandit.labs.overthewire.org -p 2220
       
      ( I used '-p' to specify the port 2220 becasue i got an error that my system was using port 22 )
      ( use password which u copied from 'spaces in the filename' file )
 <br>
 <br>
 <br>
 <br>
   <h2> All Other Levels have the same ssh connection work<br> Commands helpful in completing them are listed at the end of the writeup</h2>
 <br>
 <br>
 <br>
 <br>
 <br>
 <br>
 



<h3> Commands Learned :</h3>
    
       1) ls -a 
          - to view the hidden files , it indicates the ls to show 'all' files in the current directory.
 <br>
   
   <h3> </h3>
    
       2) cat "Password file" 
          - How to read a file which has name with spaces.
 <br>
   
   <h3> </h3>
    
       2) ls -l 
          - Displays a list of files and directories in long format and shows their sizes in bytes.
 <br>
    <details> 
   <summary>Click for picture example</summary>
   <div>
   <img width="100%" height ="370" src ="https://user-images.githubusercontent.com/91482888/190853568-d1088ff7-2f31-4f51-a06e-c704a104a714.png"/>
   </div>
    </details>
   
   <h3> </h3>
    
       3) ls -h 
          - scales file sizes and directory sizes into KB, MB, GB, or TB when the file or directory size is larger than 1024 bytes.
 <br>
 
   <details> 
   <summary>Click for picture example</summary>
   <div>
   <img width="100%" height ="450" src ="https://user-images.githubusercontent.com/91482888/190853574-2197c64b-8d09-4e19-ab49-43e1634f6010.png"/>
  
   </div>
    </details>
   
   <br>
   
   <h3> </h3>
    
       4) ls -a 
          - to view the hidden files , it indicates the ls to show 'all' files in the current directory.
 <br>
   
   <h3> </h3>
    
       5) cat ./-filename 
       
          - dash "-" is a specialm character
          - If we want to read any file whose name is starting from a dash '-' then this command is used.
 <br>
   <h3> </h3>
    
       6) find directory -size nn  ( 'find . -size +400 -print' or 'find var -size +500 -print' )
       
          - The find command enables you to search for files that fit a specific search criteria. For example, to find files that exceed a specific file 
            size, you use the following command syntax.
          - where 'directory'  specifies the directory that you want to search.
          - 'nn' is a number that represents a size in 512-byte blocks which you specify for the '–size' option.
          - The '–print' option displays the output of the find command.
 <br>
  
   <h3> </h3>
    
       7) find -type f -size 1033c 
   
          - Here type f indicates its a file.
          - b – 512-byte blocks (this is the default if no suffix is used)
            c – bytes
            w – two-byte words
            k – Kilobytes
            M – Megabytes
            G – Gigabytes
 <br>
   
   <h3> </h3>
    
       8) which  
          - An executable file (EXE file) is a computer file that contains an encoded sequence of instructions that the 
            system can execute directly when the user clicks the file icon. Executable files commonly have an EXE file extension,
            but there are hundreds of other executable file formats.
 <br>
  
 <h3> </h3>
    
       9) find / -user bandit7 -group -bandit6 -size 33c 
       
          - To find a file with given user , group and size.
          - It will open up all the files with permission and permission denied both
          - So we need to append "2>/dev/null" at the end of the above command.
 <br>
 <h3> </h3>
    
       10)  2>/dev/null
       
          - Link- https://askubuntu.com/questions/350208/what-does-2-dev-null-mean
          - /dev/null is treated as black hole in Linux/Unix, so you can put anything into this but you will not be able to get it back from /dev/null.
          - /dev/null is the standard Linux device where you send output that you want ignored.
          - Further, 2> means that you are redirecting (i.e. >) the stderr (i.e. 2) into the black hole (i.e. /dev/null).
          - Command before 2>/dev/null ill generate the output with errors and permission denied etc.
          - Specifying 2>/dev/null will filter out the errors so that they will not be output to your console.
   
          - ">" Operator:
                 *  > operator. It redirect the output of left of symbol to right of symbol.
                 *  The greater than operator ( > ) indicates to the command line that we wish the programs output (or whatever it sends to STDOUT) to be                         saved in a file instead of printed to the screen.
                 * So it must thought as : source_command > target_file
          -Every program we run on the command line automatically has three data streams connected to it:
                   0 means stdin 
                   1 means stdout(useful output)
                   2 means stderr(error message output)
          - Link: https://ryanstutorials.net/linuxtutorial/piping.php



 <br>
 
 <h3> </h3>
    
       11) strings filename | grep millionth  
       
          - To find original password after a particular word in the file as file has long data
          - Here password is found from data.txt file , password is just after the word 'millionth'.
          - notes link : https://www.javatpoint.com/what-is-linux
 <br>
   
  <h3> </h3>
    
       12) du   
       
          - Link - https://www.redhat.com/sysadmin/du-command-options 
          - Link - https://man7.org/linux/man-pages/man1/du.1.html
          - It is used to estimate the disk size a particular directory or file is using.
          - The last time it was modified (du --time)(can also specify the directory path in btwn. du and --time) etc.
          - The unit of size and other formats can be displayed using the respective flags it supports.
 <br>
   
  <h3> </h3>
    
       13) grep millionth data.txt   
       
          - The grep command can search for a string in groups of files. When it finds a pattern that matches in more than one file, it prints the name of               the file, followed by a colon, then the line matching the pattern.
          - The grep command searches through the file, looking for matches to the pattern specified. 
   
          - USE:
               type grep , then the pattern we're searching for and finally the name of the file (or files) we're searching in.
   
          - HOW IT RESULTS :
               * The grep command prints entire lines when it finds a match in a file. 
               * To print only those lines that completely match the search string, add the -x option. The output shows only the lines with the exact match.
   
          -LINK : https://ryanstutorials.net/linuxtutorial/piping.php :important concepts for commands and operator, must read.
   
 <br>
  <h3> </h3>
    
       14) file  
       
          - Link - https://medium.com/cyberdoggo/over-the-wire-bandit-534299149d29
          - Used to find the type of while, human readable or ASCII or any.
          - Wildcards like "*" etc. are used to specify the pattern or other parameters.
         
 <br>
 
<img title="find command" src="https://user-images.githubusercontent.com/91482888/223033982-313e70f8-86cb-4252-b9e6-bdacb49d2a40.jpg" width="100%"/>
 <h3> </h3>
    
       15) ls  
       
          - Link - https://www.ibm.com/docs/en/power6?topic=commands-ls-command
         
 <br>
        
   
<img title="operators" src="https://user-images.githubusercontent.com/91482888/224990467-e80c6bd3-c4b8-4faf-9cb0-6241c2d6f504.jpg" width="100%"/>   
   
 <h3> </h3>
    
       16) systemctl  
       
          - Link - https://www.liquidweb.com/kb/what-is-systemctl-an-in-depth-overview/
         
 <br>

 <h3> </h3>
    
       16) PROCESS : (Everything about PROCESSESS in LINUX)  
       
          - Link - https://www.freecodecamp.org/news/linux-list-processes-how-to-check-running-processes/
         
 <br>
   
   <h3> </h3>
    
       17)  top  
       
          -  To get the list of all the running processes on your Linux machine.
         
 <br>

   <h3>18)  "Service management" and "init (process)" :   </h3>
    
       
          -  LINK : https://www.geeksforgeeks.org/what-is-init-d-in-linux-service-management/?ref=rp
         
 <br>
   
  <h3>
    19) USER and GROUP management :</h3>
    
      https://www.redhat.com/sysadmin/linux-user-group-management
   
      https://www.ibm.com/docs/en/ibm-mq/9.1?topic=windows-creating-managing-groups-linux
   
      https://www.tecmint.com/usermod-command-examples/
   <br>
