---
layout: post
title: Contributing to the documentation of a Git Repository
---

Github doesn't support pull requests for wiki repositories. Hence it is not possible to use the traditional pull request mechanism for contributing to the documentation of a repo. Luckily, there is a workaround. The process is as follows:

Let us call the Original Repo as OLDREP.

**Step 1**: Create a new repository on your Github account. Let us call this repo as NEWREP.  <br><br>
**Step 2**: Clone the OLDREP's wiki repo to your local machine and switch to the local repo as follows:<br>  
```
git clone git://github.com/[NAME_OF_ORG]/[NAME_OF_OLDREP].wiki.git  
cd [NAME_OF_OLDREP].wiki
```
<br><br>
**Step 3**: Remove the original remote and add your Github repo as the new "origin"
<br><br>
```
git remote rm origin  
git remote add origin git://github.com/<YOUR_USERNAME>/[NAME_OF_NEWREP].git  
```
<br><br>
**Step 4**: Make changes to the documentation locally and ensure that your repo is up to date with the OLDREP's wiki repo before making the changes. Once you are done making the changes, push them to your Github repo as follows:
<br><br>
```
git push -u origin master
```
<br><br>
**Step 5**: Once you are ready to get the changes reviewed, submit the Github link of your wiki repository to the owner of OLDREP.<br><br>
**Step 6:** After reviewing the changes, the owner of OLDREP can merge the changes as follows:<br><br>
```
git clone [OLDREP].wiki.git  
```
<br>
```
cd [OLDREP].wiki.git  
```
<br>
```
git pull [NEWREP].wiki.git master  
```
<br>
```git push origin master  
```<br><br>
**NOTE** : This is only possible when the wiki changes are forked from latest wiki of OLDREP<br>
<br>

#### References: <br>
* [http://stackoverflow.com/questions/10642928/how-to-pull-request-a-wiki-page-on-github](http://stackoverflow.com/questions/10642928/how-to-pull-request-a-wiki-page-on-github)
* [http://fusiongrokker.com/post/how-you-can-contribute-to-taffy-documentation](http://fusiongrokker.com/post/how-you-can-contribute-to-taffy-documentation)