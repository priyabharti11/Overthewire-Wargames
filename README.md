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
   <h4> 
      Install Openssh client and server programs in your linux syste,m through terminal
   </h4>
   
   <h3>
    Command :
    <h4> 
      sudo apt install openssh-client & sudo apt install openssh-server
    </h4>
   </h3>
   <br>
   
   <h3> Step 2:</h3>
   <h4>
   Enable the and start the ssh service in your system.
   </h4>
   
   <h3>
    Command :
    <h4> 
      sudo systemctl enable ssh
    </h4>
   </h3>
   <br>
   
   <h3> Step 3:</h3>
   <h4>
   Now Connect to the Overwire Lab using ssh using the hostname and password given.
   </h4>
   
    <h3>
    Command :
    <h4> 
      ssh bandit0@bandit.labs.overthewire.org -p 2220<br> (I used '-p' to specify the port 2220 becasue i got an error that my system was using port 22 )
    </h4>
   </h3>
   <br>
   
   
   
   
