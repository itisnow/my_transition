SSH Access To GitHub
-----------------------

Inside this folder you have a private ssh key that you can use to directly commit your changes to this repository.
Nevertheless I recommend you create an account at GitHub.com.
In order for GitHub to generate nice statistics about contributors, you need to use the same email for your git commits as you used for the registration.
You can find some instructions on how to use this ssh key on Windows [here](https://sites.google.com/site/axusdev/tutorials/createsshkeysinmsys).
If we quickly go through them, the main steps are:

1. `SSH_ENV="$HOME/.ssh/environment"` -- create an environment file to store the info about the ssh-agent
2. `/usr/bin/ssh-agent | sed 's/^echo/#echo/' > "${SSH_ENV}"` -- start the ssh-agent. Because this is not a Windows native program we need to store the PID (process id) and and the socket number inside a file.
3. `. "${SSH_ENV}" > /dev/null` -- It is not enough to just store those variables inside a file.
We need to create some global console variables
4. `/usr/bin/ssh-add $HOME/.ssh/id_rsa_anonymous` -- finally we add the ssh key. The password is `anonymous@itisnow`.

When you use the "sudo" command in Linux it sometimes says: "With great power comes great responsibility"!

## Why the access must be open

The concept of "Pull requests" is equal to a moderator.
For code writing that could be acceptable, because code needs to work.
Ideas do not need to work and maybe they should not.
If it goes through a moderator we are limited by his knowledge.
What the moderator does not understand will not got through.
The problem is that this is the definition of innovation.
We do not understand something because it is new, which equals to innovation!
