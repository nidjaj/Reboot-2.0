## Problem 4.  share and files and folder 


#### Create two users name jack and Jill  from command line
 `- useradd jack 
  - passwd jack
  - useradd jill
  - passwd jill   `
#### Create all the data under home directory of each users 
  ` you need to login in each user account `
  
#### Login with jack user and create a file name  jack.txt using vim editor and write "hello jack"
  ` - su jack
   - vim jack.txt
  > First press i  for write
  >  In this file write
  >  "hello jack "
  > :wq  
  > for saving and quit the file `
#### From jack user also create two directories name jack1 & jack2
   ` mkdir jack1 jack2`
#### Now login from Jill user and create a file. Jill.txt using vim editor and write "hey jiil"
  ` -su jill
    - vim jill.txt
   > First press i for write 
   >  In this file we write 
   > "hey jiil"
   >:wq  
   > for saving and qit the file  `
 #### From Jill also create two directoires named jill1 & jill2 
   ` mkdir jill1 jill2 `

### Important :  swap these files and directories in between users  and to swap don't use root account.

  
