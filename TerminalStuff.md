##Terminal Commands 

#Get a Website

wget -r -np -k http://www.denishepting.de


#Server

**Connect:**

sfpt username@hostname.com 

ssh username@hostname.com


**List working directories:**

sftp> lpwd
**Local** working directory: /

sftp> pwd
**Remote** working directory: /images/


**Listing Files:**

sftp> lls
**local**

sftp> ls
**Remote**


**Uploading**

sftp> put local.profile
Uploading local.profile to /tecmint/local.profile

**Downloading**

sftp> get sampleFile.xls

**Quit connection:**

sftp> !
Shell exited with status 1


#Git

// clone it 
git clone https://www.denishepting.de


// add files
git add . (for whole directory)

git add mySuperfancy.file (for single file)

git commit -m "super fancy commit message"


//Checking settings

 git config --list
 
// For UserName or Email 

 git config user.name 
 
 git config user.email












