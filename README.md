# phpmyadmin-setup-linux-stepByStepProcess
In this repository. i have written a step to setup phpmyadmin in linux for beginners.


# Setup Process of PhpMyAdmin in Linux.

**************************** Steps and command *********************
1. To install apache2  
      sudo apt-get install apache2
2. For moving to the root directory type the command : 
      Sudo su 
3. Now to install the lamp server type the command:
     apt-get install lamp-server^

4.To install phpmyadmin type the command as :-
     apt-get install phpmyadmin –y

5. One dialog box will appear and select the ‘apache2’ by pressing spacebar.

6. Now configuring phpmyadmin dialog box will appear and select ‘yes’ after that give the password in my case it’s  ‘admin’ 🡪 This password is of ‘root   password’ 

7. Now, goto the php directory as:-
     cd /var/www/html/

8. If you hit the command as:-
      ls 
    you can see the index.html file over that directory.
9.  To see the php version you are using create info.php using command as:-
      nano info.php
 after that type the code as:-
 
   phpinfo();
 
 And press ctrl + o to save and ctrl + x to exit.

10. Now goto the browser and type ‘localhost/info.php’ you will get the php   version.

11. Then in browser go to the ‘localhost/phpmyadmin’ you will have to login    now so to create user name and password at first go to 
            sudo mysql p -u root
12. Create User using command as:
        CREATE USER 'admin'@'%' IDENTIFIED BY 'admin';
       It means that the user name is ‘admin’ and password is also ‘admin’
13. Grant Permission using the command as:-
       GRANT ALL PRIVILEGES ON . TO 'admin'@'%' WITH GRANT OPTION;
