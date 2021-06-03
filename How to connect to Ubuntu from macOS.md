
## How to connect to Ubuntu from macOS
*Once the terminal window is open and ready to go, use the apt install command to install the openssh-server package on the system.

- sudo apt install openssh-server ==> Let the packages install to your Ubuntu PC
- ssh localhost ==> Assuming the connection is successful, you will be asked to accept the SSH key. Do so.
- exit ==>  You will then be connected to the Ubuntu SSH server locally. From here, use the exit command to finish the test.


## Connect to Ubuntu from the command-line

- open Terminal
- ssh name@ubuntu-pc 
- enter password

*When the SSH connection is successful, feel free to use the command-line as if you were sitting right in front of the PC!


## How To Use The scp Command to Copy a File From Local to Remote

- scp localpath remotename@ubuntu-pc:remotepath
- enter password


## How To Use The scp Command to Copy a File From Remote to local
-- scp remotename@ubuntu-pc:remotepath localpath
- enter password
