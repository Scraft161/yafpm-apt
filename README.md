# yafpm-apt
yafpm package manager for apt.

## What is yafpm?
yafpm is a package manager frontend that does NOT reqiure the use of sudo as this is integrated inside the tool itself.
Please note that it is a frontend ONLY and this version needs to be installed on a system that has apt available eg. debian/ubuntu.

## how do i use yafpm?
### Step 1
clone the repository and type the following command.
```
sudo cp ./~/Downloads/yafpm-apt /usr/bin
```
then type the sudo password and you have succesfully installed yafpm

### Step 2
open the help menu by typing.
```
yafpm -h
```
OR
```
yafpm help
```
Note that there is no manual entry so typing
```
man yafpm
```
will symply not work.

### Step 3
Installing a package can be done by typing either of the following commands.
```
yafpm install $PackageName
yafpm -s $PackageName
yafpm grab $PackageName
yafpm -g $PackageName
```
As you can tell there are many ways to install a package

Removing a package can be done with.
```
yafpm remove $PackageName
yafpm -r $PackageName
yafpm uninstall $PackageName
yafpm -u $PackageName
```
Just as there are many ways to install a package there are many to remove one.
Also note that the -u argument uses a LOWERCASE u.

Finding packages can be done using.
```
yafpm list $PackageName
yafpm -l $PackageName
```
Note that it will find packages just like apt does.

Updating packages is done using.
```
yafpm update "$PackageName"
yafpm -U "$PackageName"
```
Note that the name of the package is not required and that it will update all packages if no name is given.
Also note that the -U argument uses an UPPERCASE u.

Upgrading is done with.
```
yafpm upgrade "$PackageName"
yafpm -UG "$PackageName"
```
Note that upgrading uses BOTH UPPERCASE u and UPPERCASE g if the -UG argument is used.

If you ever want to remove packages that are not in use by other programs you can use.
```
yafpm autoremove
yafpm -ar
yafpm purge
yafpm -p
```
Note ("No notes yet...")

And editing the sources is done with.
```
yafpm edit-sources
yafpm edit
yafpm -e
```
Note that this is exactly like in apt.

## History
yafpm started out as a joke to mock on all the different package managers and the name would describe what most poeple would think if they had to install this for one package "Yet Another Fucking Package Manager".
After that i thought i would prototype such a thing and try it out for the heck of it, But it needed its own twist: that being that it is sudoless (kind of) as the sudo was integrated inside the script and not in front of the command.
But when i ran the first prototype i realized that a sudoless package manager was great as i often forgot the sudo in front of it.
then i decided on publishing the project and making it open-source so that others can see how I pulled it of.
- Scraft161

## For developpers

If you want to help, you are free to clone or branch the project.
NOTE: if you are finished with your addition please tag your branch with "Ready" and create a pull request, I will add the code in a way that is compliant with my personal formatting rules and give proper credit, after I have done that i will reject the pull request so you can continue with development.

If you want to fork the project you are free to do so as long as a link to the original project is provided.
You do not have to credit me by putting my username in the README.md but you can if you want.
If you found a fork of my project and you want to fork that one I suggest you link both that fork and this repo (and probably others too). You are not required to do this but it insures that everyone who contributed indirectly will get proper credit.

A good copy and paste line can be
> Forked of @Scraft161 's [yafpm](http://github.com/Scraft161/yafpm-apt)
