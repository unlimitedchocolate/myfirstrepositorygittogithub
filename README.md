# myfirstrepositorygittogithub
a test repository to get used to repository functionality via git to GitHub linkage 

the first principle is to create a directory via mkdir then naming it in quotation marks "gittogithubdir" i.e mkdir "gittogithubdir"

then once you have your directory which is basically just a folder to store your files you type ls
this will list your main directories that you have as a user and among these main directories will be the directory you just created

the next part is to change the directory you are currently in to the one you just created so that you can create a file that goes inside that folder

you do this by typing cd and stating the directory you wish to go inside 
i.e cd gittogithubdir

to check you are in that directory after changing simply type pwd (print working directory) and it will tell you what directory you are in 
to see the contents of that directory simply type ls (or l -l for long list of contents)

now that you are in the newly created folder dedicated for commits to git to github you can now create a new file for this 
type touch and state the intended name of the file i.e touch gittogithubtestfile 
you have now created a file inside of your directory dedicated to git to github tasking 


the next segment is in actually getting that directories files onto the main branch of your git 
we do this by first initialising git functionality done simply via typing git init 
this commend this directory that we are currently in to the main branch of git
meaning it enables use to commit files inside that directory to git to github
i.e 
git init 
(side note if you do not have a directory you changed to beforehand git init will not work)


then we commend the file inside the directory we have chosen to the main branch 
we do this by first checking the status of the directory we are in in relation to git 
by typing git status 
it will then show the files if there are any others inside the directory in relation to git 
in terms of what is currently tracked (intended for commit) and what is not 

to set a file as intended for commit we type 
git add  i.e git add gittogithubtestfile 
it is then shown as tracked
we then issue it for commit via 
git commit -m "my first commit" or something that gives a description of that commit for the file in question 
now if we type git status
it does not show any current commits because you have already fully issued the tracked file as a commit 

now comes the syncing 

in terminal still     write git branch -M main    hit enter


write git remote add origin https://github.com/unlimitedchocolate/gittogithubtestrepository hit enter 
(you are stating the github profile you wish to sync to)

write git push -u origin main 


(git push -u origin main is the access to branch control if you typed the wrong password simply retype git push -u origin to be able to re enter password)


now you will have to put your username in
type your username ala unlimitedchocolate

then your password but since 2021 due to a security issue your password is not required, instead a personal access token is required
generate a token from your github go to  your profile image click on the down arrow icon then choose settings > developer settings > personal tokens 
generate the token 
copy your token (a key that allows you access to git branch control)
paste the token (in a safe place for later use)
paste the token in the password area
hit enter
you now have access to branch control 


to push a file found inside gittogithubdir after altering the said file 

type open gittogithubtestfile in terminal to open the file make your alterations 
then in terminal type 
git add . (add the file i just opened and altered to github repo)

the file you have just altered has been pushed along with its alterations to the github repo you created you can open the repo to check 
this concludes beginner functionality explanation of git to github    source > How to initialise and push a GitHub Repository in 2021-2022(mac)


