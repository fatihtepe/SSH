## Create a local SSH key for Mac or Linux command-line

Generate a new SSH key in your terminal called `test`. The argument provided with the -f flag creates the key in the current directory and creates two files called test and test.pub. Change the placeholder email address to your email address.

```
ssh-keygen -t rsa -C "your_email@example.com" -f ./test
```
When prompted, press enter to leave the passphrase blank on this key.


## Create a local SSH key for Windows with PuTTY

If you're on a Windows machine use Putty to generate SSH keys by following the instructions [here](https://www.ssh.com/academy/ssh/putty/windows/puttygen).
