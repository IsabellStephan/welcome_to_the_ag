## How to set up access to cluster 

write e-mail to jakob.kaminski@charite.de with your 

charite user name 

and 

github username

## Prerequisits for access to cluster

download and install Putty

https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html


## Once you get the e-mail from bih cluster refer to the wiki

https://github.com/bihealth/bih-cluster/wiki


## How to make your windows PC ready for use with unix 

You can use a linux subsystem on windows 10. See here for an instruction: 
[windows_subsystem_for_linux.md](windows_subsystem_for_linux.md).

This is useful for file transfer via command line (scp).

Alternatively you can make unix style commands on a windows PC like this:

download cygwin:

https://www.cygwin.com/


How to cygwin:

https://www.howtogeek.com/howto/41382/how-to-use-linux-commands-in-windows-with-cygwin/


## Submitting jobs to the cluster

Please first read the wiki: https://github.com/bihealth/bih-cluster/wiki and get to know the cluster. 

When accessing the cluster. Don't forget to check whether you are on a compute node. Don't compute on a login node.

Making job submission easy you should use the command qsub and a bash script that calls your actual script.

First make sure that you create a folder called logs in the correct directory, so that log files can be written to it. This is implemented in the bash scripts.

You can find a MATLAB example here:  

this ist the bash script:

[hellow.sh](hellow.sh)

it calls a silly matlab scirpt [example.m](example.m)

And here a working example for R:

this again is the bash script:

[hellowR.sh](hellowR.sh)

it calls the similarly meaningful R script [example.R](example.R)

:+1:

If you like editing the scripts on the cluster fast and like a pro :eyeglasses: you can call vim, by typing vim from the command line. Here you find some useful shortcuts. It seems a bit awkward first. But it is really fast :running:

https://www.itl.cat/wallview/xTohTR_vim-cheat-sheet/

And you have time to add emojis to your markdown scripts:

https://gist.github.com/rxaviers/7360908

For further reading on clusters, cores and nodes, here is a brief intro:

https://oncomputingwell.princeton.edu/2019/03/what-is-a-cluster-cores-nodes-slurm-cpus-oh-my/
