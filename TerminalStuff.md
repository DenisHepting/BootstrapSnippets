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
```
// 1. initialize git

git init


// 2. git status (red is uncomitted)

git status


// 3. git add ./ (whole directory) or git add README.md (file) git add -A

git add ./  git add myfile.js    git add -A


// 4. git log // shows logfile of all commited versions

git log 


// 5. git checkout 0c4e6ae // first seven digits checkout selected commit

git checkout 0c4e6ae


// 6. show current branch

git branch


// 7. create new branch

git checkout -b nameofbranch


// 8. switch to existing branch 

git checkout nameofbranch
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
