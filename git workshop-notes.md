# Git Workshop Preparing 
## Outline
- Git is a version control system
    - concept: version control (individual & group use)    
    - tools 
- Git basics
- syncing
- collaborating 
- Wrap up


## Version control is a concept/idea
### 个人使用version control的例子
	先用漫画，再用下面的例子

### 团队使用version control的例子
#### Julie
>Despite its popularity, surfing has not been recognized as a research topic in HII. Yet it has been studied outside academe for a long time by market researchers and others who have examined this behavior to help businesses to advertise their products, so potential consumers will encounter them while surfing and be encouraged to buy them. Not only are such studies proprietary, and thus inaccessible to HII researchers, they are profit-centered and as such may have very little potential to enrich the human-centered understanding of the phenomenon which motivates HII research. 
>>Experiment Data: 
>>>Akddshfhh  
dDjkfdhjd  
Djkfhsod  
jdsfhjf

#### Cody
>Despite its popularity, surfing has not been recognized as a research topic in HII. Yet it has been studied outside academe for a long time by market researchers and others who have examined this behavior to help businesses to advertise their products, so potential consumers will encounter them while surfing and be encouraged to buy them. Not only are such studies proprietary, and thus inaccessible to HII researchers, they are profit-centered and as such may have very little potential to enrich the human-centered understanding of the phenomenon which motivates HII research. 
>>Experiment Data: 
>>>dslfdjjdksjfddfdsfdsssdsfsdfs
	dkjfsdlkfjdsffffffffffffeffff
	kdlsjfldskjfsssssssefsafeasfeawfe
    dsflkjsdfssafdsfdasfdasfsefewfew

- Whoever upload the version later, is the most updated version. 

## Functions of version control
- Collaboration - Version control helps teams work collaboratively on same set of documents without interfering with each other. 协同修改  
- Rolling back - Made a mistake? Version control lets you review and undo changes, reverting to previous stages in the document’s history. This can be useful when changes to your files introduce unforeseen problems.  数据备份  
- Versioning - It provides a thorough log of changes to tracked files without creating multiple copies, making it easier to identify the most current version. 版本管理  （这方面SVN 使用增量式管理，Git采用文件系统快照 snapshots）  
- Understanding context - help you understand how the code or writing came to be, who wrote or contributed particular parts, and who you might ask to help understand it better. 了解历史演变  
- Backup - While not meant to be a backup solution, version control systems mean your code and writing can be stored on multiple computers. 可以在多台电脑储存你的数据  
- Access Control -  give different levels of accessibility to members of the group; Non-group members can contribute and the content can be checked and merged in (Git exclusive)
- Branch management   


## Version control systems are the tools we can use to realize the concept

### Centralized version control system：CVS, SVN, VSS…

<picture 1>

### Distributed version control system：**Git**, Mercurial, bazaar, Darcs…
 
<picture 2>

## Git Workflow on your computer
the (git) repository  （history versions)
-- git commit  
the staging area or the index/cache  (temporary storage)
-- git add  
the working area or the working tree (coding)

<picture 3>  
Practice!  
pre-workshop set up: installation, signature, text editor

zsh - bash  
`chsh -s /bin/zsh`

1. creating a repository  
`git init`  
.git  
`git status`  
`git add`  
`git commit -m ""`

### GitHub: hosting remote repositories
1. internal collaboration
2. external collaboration

## Git and GitHub Script
### Introduction
Hello everyone, welcome to the Git and GitHub workshop. This workshop is offered to you by UBC library research commons. 

Before beginning the workshop, I’d like to acknowledge that UBC Vancouver is on the traditional, ancestral, and unceded territory of the Musqueam people. I encourage you to learn more about what it means to be here on this territory.  You can start learning about th history of th land at https://indigenous.ubc.ca/indigenous-engagement/musqueam-and-ubc/ and continue to learn more.

My name is Billie, I am a graduate academic assistant at research commons. I am also a current graduate student studying library and information. 

I would like to remind everyone that this is a workshop that encourages your active participation. We expect you to type out the command lines and open websites on your end with me because just listening is not a very effective learning strategy. In the meanwhile, if you have questions, you are welcome to communicate with me o my colleague Jerin in the chat. I will try my best to answer your questions.

Let’s try the reactions out. Can everyone tell me have you done the pre-workshop set up? 

If you do not have the set up ready, my colleague Jerin is going to send instructions in the chat. You can do that while I introduce the concepts. 

For those who are fully ready for this workshop, thank you. I am going to introduce you some key concepts of Git and GitHub and our goal is to begin to understand and use Git and GitHub. You will not be an expert by the end of the class,  probably not even feel very comfortable using Git. This is okay. We want to make a start but, as with any skill, using Git takes practice. And we want you to start practicing right from our workshop.

One-on-one zoom consultation (link)
![image](https://user-images.githubusercontent.com/95002283/151864079-767028a6-317a-47d2-919d-15ad1471cbc2.png)


## Functions of version control
- Collaboration - Version control helps teams work collaboratively on same set of documents without interfering with each other. 协同修改  
- Rolling back - Made a mistake? Version control lets you review and undo changes, reverting to previous stages in the document’s history. This can be useful when changes to your files introduce unforeseen problems.  数据备份  
- Versioning - It provides a thorough log of changes to tracked files without creating multiple copies, making it easier to identify the most current version. 版本管理  （这方面SVN 使用增量式管理，Git采用文件系统快照 snapshots）  
- Understanding context - help you understand how the code or writing came to be, who wrote or contributed particular parts, and who you might ask to help understand it better. 了解历史演变  
- Backup - While not meant to be a backup solution, version control systems mean your code and writing can be stored on multiple computers. 可以在多台电脑储存你的数据  
- Access Control -  give different levels of accessibility to members of the group; Non-group members can contribute and the content can be checked and merged in (Git exclusive)
- Branch management   


### set up 
chsh -s /bin/zsh  (change a login shell)

git config -–global user.name 
	         user.email

git config -–global core.editor “notepad”

pwd (print work directory)
ls -a
cat .gitconfig  (cat is a standard Unix utility that reads files sequentially, writing them to standard output. The name is derived from its function to concatenate files.）

Give the gitpage for reference

### practice
mkdir
git init
touch test.txt  (create)
git add
git commit
cat test.txt
Nano test.txt  

练习几次 add 和 commit  然后休息5分钟  
#### check differnence
nano test.txt      'check difference'    
mkdir test-directory  
git diff  

The dit diff command shows the changes we have made before a commit.   
Line 1 tells us Git is comparing “a” and “b” versions of the index.md file  
Line 2 indicates which tracked versions “a” and “b” correspond to; “aed0629” and “989787e” are unique computer-generated identifiers for each version  
The last two lines show the changes to the “index.md” between the compared versions:   
there were no changes to the.... line  
a line was added with the text ... (“+” indicates an addition and “-“, a deletion)  
We can now add and commit the updated version of “index.md”:  

#### check log
git log  
git log --pretty=oneline  
git log --oneline  
git reflog  

git log lists information about all commits in reverse chronological order, including the commit messages we wrote to describe them. It is important to add meaningful commit messages, especially when working on teams. Best practice is to write commit messages in the imperative (e.g. ‘Add index.md’ instead of ‘Adding index.md’).  

#### back and forth
git reset --hard ae90djke  
git reset --hard HEAD^  
git reset --hard HEAD~n  
//hard: resets the index file and git repository 暂存区+本地库  
//mixed: resets the index file not git repository 暂存区  
//soft: do not touch the index file or working tree 工作区  

git reset --mixed dkdh39  
git reset --hard HEAD   //use this to sync the git repository with the index file  

### syncing with GitHub
create repository  
create 
$ cd ~  
$ ssh-keygen –t rsa –C [your GitHub email]  
$ cd .ssh  
$ ls  
$ cat id_rsa.pub  
$ (copy and paste to GitHub)  

rm -rvf .ssh  

For every action that you perform, SSH removes the burden of authenticating on your remote server for every action (clone/push/pull) in git. This is one of the major reasons why SSH prefers to HTTPS. ... SSH seems to be more secure than HTTPS as it does not use password-based authentication.  

git push origin master  

git remote rm origin  

#### pull
When working with others or on multiple computers we need a way to pull all the remote changes back into our local repository. We can see how this works by adding a file to our GitHub repository, then “pulling” that change back to our computer.  

Near the bottom of the “hello-world” repository on GitHub there is a button to “Add a README” file to your repository. Click the button, enter some text, then scroll to the bottom and click “Commit new file” (The default commit message will be “Create README.md”, which is fine for our purposes).  

It is good practice to add a README file briefly describing what the project is about. If the README is in the root directory GitHub will automatically display it like a cover page for your repository.  
After adding a README on GitHub your local repository is out-of-sync with the remote repository. Let’s fix that by pulling the remote changes into local repository with git pull.  
git pull origin master  




