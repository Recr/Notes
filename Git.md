Git is a free [[Open Source|open-source]] Distributed Version Control System. It is light-weight and quick and have efficient branching and merging features.
###### Brief history
In 2002 the open-source Linux Kernel project workers started using a proprietary DVCS called BitKeeper. After conflicts with their community, in 2005, BitKeeper decides to terminate the free license, forcing Linus Torvalds (Linux Kernel creator) and his team to migrate to another software, and he decided to create his own software, Git.
###### Basic Flow
In the start of an project, someone will create a repository with ```git init``` in a server or locally and push (send) to the server. To do that, we use ```git commit``` to save the changes locally and ```git push``` to send it to the server.
After that people can clone the repository in the server using ```git clone``` and retrieve the alterations with ```git pull```. 
It has an official [site](https://git-scm.com/) where one can download the software and also have access to the documentation that explains how it works.
### Git configuration
In Git we can configure lots of options with the command ```git config```, and also there are three scopes in that regard that we can choose: system, global and local. Changing an option in the system scope means that for every user that uses the computer, the changes will take effect. Changing an option in the global scope, takes effect for the current user of the system, not all of them, and finally the local scope changes options for an specific repository or project.
For example we could use a command to change the username in Git, and do that in the global scope so the current user will use the specified username for every repository. For that we would use the following command:

```git
git config --global user.name "new username"
```

To change the default branch name globally we would use:
```git
git config --global init.defaultBranch
```

We can use this command to list every change we've made thus far:
```git
git config --global --list
```

Initially we want to set the username and email and with just that we could already use Git, but just locally in our computer. But what if the necessity to work with remote repositories surges? That's where [[GitHub]] enters.
In order to link Git and GitHub we need to establish a connection between then. Until 2021 we could just use the user and password from a GitHub account, but due to security issues, GitHub now works with credentials.
We have the option to connect via a randomly generated token with determined validity or through a SSH key, that serves as a kind of cryptographed passwords. 