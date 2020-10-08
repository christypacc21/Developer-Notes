---
description: Professional conducts that protect your codebase
---

# Working in a team using Git

### \[Commiting code\]

* **Write understandable and meaningful comments while committing** 
  * For example, "Added README.md" instead of "kjhaksdfhkasdfhjk".



* **Create a branch and merge back to the main branch through a Pull Request**
  * The best and most secured way to make a GIt commit is to create a branch out of the main branch \(the main branch could be any branch, for example, the master branch, the development branch, the staging branch, etc, depending on your task\) and make changes and commit in the newly created branch. And then make a pull request _\(i.e. a request to code reviewers \(eg your tech lead or teammates\) for approving your new branch's code to be added into the main branch's code\)_ back to the main branch. 
  * Skipping this step is still acceptable for small teams \(eg under 3 people\) if they need to move fast. However, if it is a big team, then it is a must to do to secure the codebase. In my workplace, I worked on projects that had over 10 million users and developers were required to do so even if we were just changing a single line of code.



* **Add unnecessary-to-be-committed or confidential files to ".gitignore"** 
  * Add all these files in ".gitignore", so that the information will not be included in the commit. Also, for Node.js developers, always remember to .gitignore "node\_modules" folder.



* **Double-check to ensure no confidential credential \(eg secret keys, passwords\) is included in the commit.** 
  * If you really need to store keys in your code, create a local \(local means will not be committed\) config file \(eg secretKey.js\) and add its name to ".gitignore", and then create a sample public file \(eg secretKeySample.js\) with the equivalent schema of content in it, so that other developers can create their own local secretKey.js following your secretKeySample.js schema. This method makes the credentials never show in the cloud codebase, preventing hackers or unrelated parties from knowing the credentials by looking at your codebase.





