# Git-Command-Guide
All use case available of Git &amp; Github


# Heading 1
## Heading 2
### Heading 3

`text red ` 

*Italic* or _Italic_

**Bold** or __Bold__

* Item 1
* Item 2

1. First item
2. Second item

[Google](https://www.google.com)

![Alt Text](image-url)

---
or
***

| Header 1 | Header 2 |
| -------- | -------- |
| Content 1| Content 2|

$$ E = mc^2 $$

# My Markdown File

This is a paragraph of text in my Markdown file.

## Code Example

Here is a code block:

```javascript
function greet(name) {
  console.log("Hello, " + name + "!");
}

greet("World");

```
```python
print("hello world")
```
# Git Comonds
## Git
Version Control System is a tools that to track changes in code.<br>
`Git is a Version Control System `

## Github
Website that allow developer to store and manage their code using Git

##  Configuring Git 
```git 
git config --global user.name "myName"
git config --global user.email "email@gmail.com"
git cofig --list
```
## Create repo using clone comond in git

```git
git clone <- repo http link ->
```

make some changes (modefied => changed) or create new file (untracked)
```git
git status
```
Output :- modefied => changed , untracked file

### Staged

```git
git add fileName 
```
or 

```git
git add .
```

```git
git status
```
Output :- staged

### Commit
```git
git commit -m "commit message"
```

```git
git status
```
Output :- Unmodified (Unchanged) or up to date

### Push Code on Github

```
git push origin <branch>
```
### Create new branch
```bash
git branch branch_name
```
Creates a new branch but does not switch to it.
```bash
git checkout -b branch_name
```
Creates a new branch and switch to it.

### Switch branch

```bash
git checkout branch_name
```
switch to given branch.

### Delete branch
```bash
git branch
```
O/p :- list of branch <br>
for example<br>
main<br> 
*UI_dev_1 <br>
UI_dev_2 <br>

```bash
git branch -d main
```
```bash
git branch -d UI_dev_2
```
you can not delete current branch (UI_dev_1)

```bash
git push origin -d branch_name
```
### Merge branch
```bash
git branch
```
O/p :- list of branch <br>
for example<br>
main<br> 
*UI_dev_1 <br>
UI_dev_2 <br>

```bash
git diff branch_name
```
 To compare commits, branches, files & more
```bash 
git merge main
git checkout main
git push origin main
```
or
```bash 
git merge UI_dev_2
git checkout  UI_dev_2
git push origin  UI_dev_2
```

### Create a PR
It lets you tell others about changes you have pushed to branch in a repo on GitHUb.

### Pull Command
```bash
git pullo origin main
```
Used to fetch download content from a remote repo and immediatly update the local repo to match that content.

### Unding Changes 
#### Case 1 :- staged changes
```
git reset <- file_name ->
or
git reset
```
#### Case 2 :- commited changes (for one commit)
```
git reset HEAD-1
```
#### Case 3 :- commited changes (for many commit)
```
git reset <- commit hash ->
or
git reset --hard <- commit hash ->
```
### Fork
A fork is a new repo that share code and visibility settings with the original "upstream" repo.<br>
`Fork is a rough copy`





