- #  1 owner of file
 - owner of file is  **the user who created the file**
#user and  #group 
**User groups are a collection of users who perform a similar task**
1. #user *associated with a user account, which consists of several properties*
2. #group  *it a collection of users
#### we can change the owner of file using `chow`

#### syntax to change owner
`chown username:Groupname filename`
1. **we can change booth in one**
`chow username:groupname filename`
2. we can change only user
 `chow username filename `
3. **we can change only group**
  `chown groupname: filename `
#  2 Permission of file
##### Every file contains three permission this 
1. **Read** (r)
2. **write(w)**
3. **excite (x)**
## in permission it have 3 things
1. **User (o)** it contains the main user 
2. **Group (g)** it is contains group of user
3. **Other(o)** it is other user 
#shortkey 
**all user (a)**
**Give permission we use(+)**
**Remove permission(-)**
## we can change file permission using `chmod`
### 1 Give Access
- `chmod a+rwx file name`*used to give all  permission for user group and other*
- `chmod +rwx file name` *used to give permission for all using default*
- `chmod u+rwx filename` *used to give permission for only user
- `chmod g+wrx filename` *used to give permission for only group*
- `chmod o+wrx filename ` *used to give permission for only other*
### 2 Remove permissions 
- `chmod a-rwx file name`*used to Remove  all  permission for user group and other*
- `chmod -rwx file name` *used to Remove  permission for all using default*
- `chmod u-rwx filename` *used to  Remove permission for only user
- `chmod g-wrx filename` *used to  Remove permission for only group*
- `chmod o-wrx filename ` *used to  Remove permission for only other*

 
