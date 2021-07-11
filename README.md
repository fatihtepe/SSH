## easy SSH 
[Programmers: Learn More SSH](https://medium.com/for-linux-users/programmers-learn-more-ssh-d2985f1a6063)

The concept is very simple. You create a public/private key pair on your home machine and put the private key in a secure location. Then you log into a server once using your password and deposit the public key in a place that ssh knows to look.
Now when you try to log on, ssh will notice the public key and encrypt some data using it. Remember, sharing your public key with people has no real risk. That’s why it is a public key.

[Easy SSH Authentication](https://at0dd.medium.com/easy-ssh-authentication-7151303189a3)

If you’ve ever used SSH to remote into a server, you’ve had to type your password a few times. Setting up a SSH key creates a trust between your local computer and your server, allowing you to login without having to type your password. Below are step-by-step guides for creating a SSH key on Windows and macOS/Linux.
