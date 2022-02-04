## Git work results

---
- I created a <ins>develop</ins> branch and **index.html** in it
- Then, I created a branch called <ins>images</ins>
- On this branch, I created a folder with two images and added their sources to **index.html**
- Then, I created a new branch <ins>styles</ins> from <ins>develop</ins> branch
- After that, I created a folder with some styles and changed **index.html**
- The next step was to merge branches (<ins>images</ins> and <ins>styles</ins>) to <ins>develop</ins> branch
- Ran commands: `git checkout develop` `git merge images`. They successfully merged. 
- Ran command `git merge styles` and got a conflict error. That because the content of **index.html** was differing on 
<ins>develop</ins> branch and styles one
- Resolved conflict and made a commit 
- Ran a command `git reflog` and saved the result to **task1.1_GIT**

## What is DevOps?

---
This is a kind of developing direction which helps to adjust work between programmers and people who are responsible for
the project's administration. DevOps technology helps to enhance stability and provide a reliable connection.
