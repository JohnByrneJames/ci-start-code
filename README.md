# Why should we use SSH with Git-hub

## SSH keys and Git-hub
### There are two methods to clone the repo

``` SSH AND HTTPS ```
- We have two types repos ```public repo``` 
- second is ```private repo```

**Generating a SSH Key**
- generate the SSHkey your local system 
- copy the key from the local system to the specific on GitHub
- On this occasion That Repository is called [ci-start-code](https://github.com/JohnByrneJames/ci-start-code)
- .ssh folder where we store the ssh keys available
- Name the key as your name (E.G. John)

- To see the folder you need to go to the users/user in your C:/ drive and type `ls -a` to view the ssh key folder
- Go to users, and your user then look for the `.ssh` folder
- Enter the folder using `cd .ssh`
- Then I entered the following command `ssh-keygen -t rsa -b 4096 -C "my_email" `
- Then I entered my name as the key `name` and left the passphrase blank.
- Now I copy the public key with the command `cat john.pub`

- Go to the gitHub repo > Settings > Deploy Keys and add a new key with your name as the title
and the public key with the one you just copied.

## It is essential and best practice to give the keys a descriptive name

In this case we just called it our names for testing purposes but it can be good to name it with the software it is being used with. For example "Name"-"Software" (E.G. John-Jenkins)

- Now the secured public key from our local system has been copied to our cloud which is GitHub in this case.

