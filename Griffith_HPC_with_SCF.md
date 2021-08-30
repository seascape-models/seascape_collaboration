# Using the Griffith HPC with the SCF

This guide assumes you have a good understanding of git command line interface (CLI), GitHub and the Griffith HPC (and already have accounts setup).

## Password-less login to the HPC

You need to have a working ssh key set up (with no passphrase). To do this follow the multi-page instructions [here](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent). Once your ssh key is full setup go inside the "./ssh" directory on your computer (or create this based on your operating system) and add a file called "config" with no extension with the contents (sXXXXXX is your Griffith username): 

```
Host ghpc
    HostName 10.250.250.3
    User sXXXXXX
    IdentityFile ~/.ssh/id_ed25519.pub
```

After doing this logon to the Griffith HPC with the in terminal or putty using the command `ssh ghpc`. Then, use the command `nano ~/.ssh/authorized_keys` and copy the contents of your **PUBLIC** key from your computer (~/.ssh/id_ed25519.pub) as a new line in this file. Hooray!.. you are now setup to logon password-less to the hpc, with command `ssh ghpc`.

## Using git and GitHub on the HPC

You cannot use the Github desktop app on the HPC (as far as I know), so you have to use the CLI. This, requires a more in depth understanding of git and GitHub (but is useful and not "too" hard). You also have to use https origins because ssh ones are disabled on the HPC. The main things you need to understand and know how to use are:
```
git clone
git fetch
git commit -m""
git add
git status
git push
git pull
```
## Work flow

1. Make changes to project on your computer and push to GitHub
2. Transfer files you need in the "Shared" folder to the projects "Shared" folder on the HPC using a file transfer system (do NOT transfer files tracked by the git repository)
3. Login to the Griffith HPC
4. Run command "source s3proxy.sh" in the terminal
5. Go inside the directory of your project with "cd ~/" like commands (or git clone by https:// if the repository is not yet on the HPC)
6. Pull from GitHub
7. Run your script on the HPC
8. If you made changes to code on the HPC, commit them and push using the CLI
9. Transfer script outputs to the "Shared" folder on you computer
10. DONE

## Other tips and tricks

* Have a proper [directory structure](https://github.com/seascape-models/seascape_collaboration#directories-and-files), on the HPC like you should in any other location.
* Generally speaking, make changes to your code on your computer rather than on the HPC so you can avoid having to 'git add .', 'git commit -m""' and 'git push', and instead only need to 'git fetch' and 'git pull'
* Just transfer the files you need from in the "Shared" folder.