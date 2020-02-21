# midterm

### First section: You must explain the difference between cloning vs fetching vs pulling. Give real world examples of how they differ.
Cloning a repository is essentially making a copy duplicate of someone else's source code. It also allows the user to set up their own local branch. It can create a remote called 'origin' for the repository it was clones from. It sets up its own local branch based upon the remote's active branch. An example of the purpose of cloning is that if it is an open source project, the clone repo could point back to the original repo and because there is a local branch that gets created, it has a connection to the original. The reasons why a user would clone a repositiory is to contribute back to organiziaiton projects and make use of open source repositories.

Fetching refers to when it gets all the new changes (if any) from the master branch. It does not do any merging to the master branch. Git fetch is the command to let your local git retrieve the latest data from the original. An example of fetching in a real-life situation is if you're on a team and each person is working on a component. The code reviewer would look if there are any merge conflicts to the master branch before their merge and accidentally overwrite any particular code or file that might conflict with someone else on the same team.

### Second section: Create a markdown table that shows the basic differences between Trello and Asana. The list does not need to be exhaustive. Make sure to use a table.
| Trello     | Asana |
| ----------------------- | ------------------------------ |
| Kaban Board only |List, Board, Timeline, Calendar, Files, Progress, Portfolios, Workload, Inbox, My Tasks|
|does not have progress & reporting |advance search options, reports, milestones, project progress |
| no work prioritization | has work prioritization |
| mimics real-life boards to manage the project | takes a task-oriented approach |

### Third Section: Answer the following 3 questions:
#### Question 1: What is the .git folder? Where is the object database in this folder?
The .git folder is a hidden folder and it contains all the information necessary for th e project's version control. It is set up with files and directories. It also stores the config folder (core settings) and refs folder. It holds information about commits, remote repository address, a log that stores the commit history so that you are able to roll back. 

#### Question 2: Explain in detail how the git hash-object function works. 
The git hash-object creates new (BLOB) objects in git and add it to the git database. These are also one way functions and are created based upon a given input. It cannot be converted back to its original input. It also does have a fixed length (based on the hash function used) for its output (also known as hash values) regardless of the input length. Hash functions will always generate the same hash values with the same given input. There are also an array of hash functions like: MD5, SHA1, SHS256. If the hash function used is MD5, the hash value will be a 32 digit hexadecimal with a value of 128-bit.

#### Question 3: Where does git internally store the file names to our files? How are tree objects related to this?
Git compresses and stores each time a file is created in its own data structure. The compressed object will have a unique name, a hash, and stored in an object directory (tree objects). Tree objects are the way git represents its directories. Each tree can contain a BLOB and other trees and links to them as well. When a file gets created, and since the update-index is built-in it already gets added in regardless if it is a BLOB or not.
