##Terminal Commands 

#Get a Website
```
wget -r -np -k http://www.fancywebiste.de
```
#Server

**Connect:**
```
sfpt username@hostname.com 

ssh username@hostname.com

```

**List working directories:**
```
sftp> lpwd<br>
**Local** working directory: /

sftp> pwd
**Remote** working directory: /images/
```

**Listing Files:**
```
sftp> lls
**local**

sftp> ls
**Remote**

```
**Uploading**
```
sftp> put local.profile
Uploading local.profile to /tecmint/local.profile
```
**Downloading**
```
sftp> get sampleFile.xls

```
**Quit connection:**
```
sftp> !
Shell exited with status 1
```

#Git

##Basics

**Initialize git**
```
git init
```

**Git Status**
```
git status
```

**Git add (file or whole directory)**
```
git add ./  git add myfile.js    git add -A
```

**Git log (shows logfile of all commited versions**
```
git log 
```

**Git checkout (branchname or first 7 digits of commit you want to use)**
```
git checkout branchname

git checkout 0c4e6ae
```

**Show current branch**
```
git branch 
```

**create new branch**
```
git checkout -b nameofbranch
```

**switch to differnent branch**
```
git checkout nameofbranch
```

## Remote stuff

You need a ssh key for github to use these with your profile

**list remote connections of repository**
```
git checkout nameofbranch
```

**add new remote origin**
```
git remote add origin git@github.com:YOUUSERNAME/YOURREPOSITROY.git
```

**remove a origin in case you want to change it**
```
git remote rm origin 
```

**pull from remote**
```
git pull origin branchname
git pull origin master

// If problems with pull
git pull origin branchname --allow-unrelated-histories
```

**push**
```
git push origin branchname
```

// clone it 
```
git clone https://www.denishepting.de

```
// add files
```
git add . (for whole directory)

git add mySuperfancy.file (for single file)

git commit -m "super fancy commit message"
```
//Checking settings
```
 git config --list
 ```
// For UserName or Email 
```
git config user.name 
 
git config user.email 
```

## Airport Stuff

```
List Wifi Devices
airport -s
```

http://www.saltwaterc.eu/capturing-wpa-handshakes-with-os-x.html
https://gist.github.com/victorreyesh/6532800


# General Commands 

```

// change directory
cd 

// create directory
mkdir

// create file
touch myfile.html 

// open file in vim Editor
vim README.md

//ESC, shift colon to save file

// show calendar 
cal 04 1990
```

## NPM 
```
// List all global packages
npm ls -g --depth=0 

// Uninstall global packages
npm uninstall -g nameofglobalpackage

sudo unistall -g nameofglobalpackage

// install globally
npm install -g gulp

npm install -g nameofpackage
```
