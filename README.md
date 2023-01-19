# Linux
Linux Learning
Terminal: Its a kind of app that handles the input from user and displays the output . For example : In Mac os we have iTerm2 or in windows its putty.
Shell : Its a command line interface. It provides an interface between the user and the kernel and executes programs called commands. 
The Shell is the name of the program that runs in the terminal 
Types of Shell : Bash Shell , ZSH shell . 
How to check which shell are we using : echo $SHELL.
echo is like print statement , it will show the value for the arguments passed here as a input like $SHELL(means get the value of SHELL command)
Once we open Terminal it will have option like this :
[root@ins-dm-gjtestmysql101z ~]# ==> So basically here root is the user on server , @ is seprator and ins-dm-gjtestmysql101z is the hostname of machine .
Hostname is basically the name of server by which it will be called in the network . It can be viewed using the command : hostname.
Scenario: Lets say if am running python3 command , how does system will understand if its executable or its a file . Basically behind the scene it run 
the commmand "where python3 " and it will be execute then ==> where python3 (o/p =Note − /usr/local/bin/python3 is the path of the Python directory.)
ls : list of files in present working directory
ls -a : Show all the hidden files in the directory
pwd: present working directory 
Once i open a new directory it will by default point to my home directory i.e /Users/kriti
Whatever command i will run , it will execute in the same folder where currently i will be pointing to 
mkdir test : Create a new folder with test name
cd test: Change current working directory/folder to test folder
cd.. : To get one folder back from current working directory
Environment variable in linux : Environment variables allow to customize how the system works and the behavior of the applications on the system. 
echo $PATH : It specifies the directories to be searched to find a command . like if we run python3 command it is going to search that executable command 
in each of the location specfied in PATH Env variable.
cat ~/.bashrc. ==> Cat displays the content of a file . So basically here it means to open display the content of bashrc file located in home directory
bashrc is a file that will automatically be loaded once a interactive terminal open . So all kind of env variable settings or alias setting we store here
alias : Alias in shell means to set short names for a long command like [alias a="docker run nginx"] . Now if we run "a" then it will call "docker run nginx"
Now to set environment variable in shell we need to use export command like [export mysql_password="my-secret-pw"]. This will only be valid for a particular
terminal session . If you need change permanent then make change in bashrc file as explained above .
echo $mysql_password ==> Will give value of mysql_password variable.
cat > file.txt. ==>Creating and writing to the same file 
My name is kriti and to do exit press (ctrl+c)
Now see content of file.txt , it will show the content as "My name is kriti"  


Assignments:
1. get hostname of your machine
2. Export two variables named as MY_SQL_USER and MY_SQL_PASSWORD
3. Echo the two variable values
4. Export the above two variables in bashrc file.
5. List all hiddden files in your home directory.
6. Create a directory in your home folder named as test and inside the test folder create file my_intro with content as your name.
