# GitHub
For github some code 

How to all repository make private or public???=====>

 1) curl --request GET https://api.github.com/users/abc/repos  abc=yourUsername for github get request with command to see your all of repository in cmd
 late go to your github =>settings=>DevelopperSettings=>Personal access tokens=>generate new token
 wrtie not something select scopes 
 1.repo 2.admin:public-key 3.delete repo 4. project 5. admin:gpg_key ==== or all of tick    =>>> next
 
 2) curl -u abc:TOKEN --data "{\"private\": \"true\"}" --request PATCH https://api.github.com/repos/abc/xyz
 for one repo make e private or public ===> private true or false
 
 1.abc==your username for github
 2.Toke== past your generating token 
 3.in the url abc=your username for git 
 4.xyz= your repo name 
 
3) curl -u abc:TOKEN --data "{\"private\": \"true\"}" --request PATCH https://api.github.com/repos/abc/%
 
 also here 
 1.Toke= your generatin token
 2.abc= your username 
 3.change the url abc=your username for github and % for all repository make private or public
 
 
 How to delete appsettings.json file for project
 
 git rm --cached project/appsettings.json
 and commit it and push
