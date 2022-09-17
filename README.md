# Overthewire-Wargames

Overthewire Wargames is a platform for prcaticing Security Concepts in the form of fun filled games.

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
   <h3></h3>
       1) ls -a 
          - to view the hidden files , it indicates the ls to show 'all' files in the current directory.
 <br>
   
   
   
   
