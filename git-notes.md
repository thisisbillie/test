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

- Despite its popularity, surfing has not been recognized as a research topic in HII. Yet it has been studied outside academe for a long time by market researchers and others who have examined this behavior to help businesses to advertise their products, so potential consumers will encounter them while surfing and be encouraged to buy them. Not only are such studies proprietary, and thus inaccessible to HII researchers, they are profit-centered and as such may have very little potential to enrich the human-centered understanding of the phenomenon which motivates HII research. 

The closest concept to surfing that has been investigated in HII is what Savolainen (1995) called “seeking of orienting information.” He defined orienting information as information “concerning current events,” in contrast to practical information, “which serves as the solution to specific problems” (Savolainen 1995, 272). The purpose in seeking of orienting information, Savolainen argued, is to create a passive habitual moni- toring system to focus on everyday matters by asking: How are things at this moment? Thus, while they are related, seeking of orienting information differs from surfing by defi- nition. One other recognition of surfing is its entry in the Online Dictionary of Library and Information Science (Reitz 2007), which explains that to surf is to navigate the web with no definite purpose in mind. To date, the area of surfing—that is, browsing with no specific informational purpose—remains uncharted by HII researchers and ready for exploration. 

- Update different versions but go back to any of the previous versions in a clean, easy, and accurate way.


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
Rolling back - Made a mistake? Version control lets you review and undo changes, reverting to previous stages in the document’s history. This can be useful when changes to your files introduce unforeseen problems.  数据备份
- Versioning - It provides a thorough log of changes to tracked files without creating multiple copies, making it easier to identify the most current version. 版本管理  （这方面SVN 使用增量式管理，Git采用文件系统快照）
Understanding context - help you understand how the code or writing came to be, who wrote or contributed particular parts, and who you might ask to help understand it better. 了解历史演变
Backup - While not meant to be a backup solution, version control systems mean your code and writing can be stored on multiple computers. 可以在多台电脑储存你的数据
Access Control -  give different levels of accessibility to members of the group; Non-group members can contribute and the content can be checked and merged in (Git exclusive)
Branch management 


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

Before beginning the workshop, I’d like to acknowledge that UBC Vancouver is located on the traditional, ancestral, and unceded territory of the Musqueam, Tsleil-Waututh, sha-main-us, Stó:lō, Squamish, and Coast Salish peoples.

Let me introduce myself. My name is Billie, I am a graduate academic assistant at research commons. I am also a current graduate student studying library and information studies. 

I would like to remind everyone that this is a workshop that encourages your active participation. We expect you to type out the command lines and open websites on your end when I tell you so because practicing is not the same as just listening. In the meanwhile, you are welcome to communicate with me in the chatbox or simply give me reaction by clicking different icons.

I am going to introduce you some key concepts of Git and GitHub and our goal is to begin to understand and use Git and GitHub. You will not be an expert by the end of the class. You will probably not even feel very comfortable using Git. This is okay. We want to make a start but, as with any skill, using Git takes practice.





