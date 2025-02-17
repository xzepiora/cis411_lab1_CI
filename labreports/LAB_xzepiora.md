# Lab Report: Continuous Integration
___
**Course:** CIS 411, Spring 2021  

**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  

**Name:** Xavier Zepiora

**GitHub Handle:** xzepiora

**Repository:** cis411_lab1_CI
___

# Step 1: Fork this repository
- The URL of my forked repository: https://github.com/xzepiora/cis411_lab1_CI
- The diagram below illustrates how a fork works.
  ![Forked Repo](./Images/Lab%20Requirements%20(4).jpg)



# Step 2: Clone your forked repository from the command line  
- My local file directory is C:\Users\seadr\OneDrive\Documents\GitHub
- The command to navigate to the directory when I open up the command line is cd cis411_lab1_CI

# Step 3: Run the application locally
- My GraphQL response from adding myself as an account on the test project
``` json
{
  "data": {
    "mutateAccount": {
      "id": "648b852f-13ec-4263-8f21-33af9ba77988",
      "name": "Xavier Zepiora",
      "email": "xz1151@messiah.edu"
    }
  }
}
```

# Step 4: Creating a feature branch
- The output of my git commit log
```
e661bd1 (HEAD -> labreport, origin/labreport) @trevordbunch
94babae (upstream/purelab, upstream/HEAD, origin/purelab, origin/HEAD, purelab) Merge pull request #59 from JeffSinsel/purelab
2e92bd8 Fixed typos and links in markdown files
fa4fc85 Update Instructions
f8513e0 Update Node links to Instructions
d4f22eb Update repo branch names
0e3ae4c Reset purelab
050b420 Merge pull request #2 from trevordbunch/main
1fe415c Merge pull request #1 from trevordbunch/labreport
13e571f Update Lab readme, instructions and templates
eafe253 Adjust submitting instructions
47e83cd Add images to LabReport
ec18770 Add Images
dbf826a Answer Step 4
a9c1de6 Complete Step 1, 2 and 3 of LAB_TREVORDBUNCH
1ead543 remove LAB.md
8c38613 Initial commit of labreport with @tangollama
dabceca Merge pull request #24 from tangollama/circleci
a4096db Create README.md
2f01bf4 Update LAB_INSTRUCTIONS.md
347bd50 Update LAB_INSTRUCTIONS.md
7aaa9f3 Update LAB_INSTRUCTIONS.md
37393ae Bug fixed
1949d2a Update LAB_INSTRUCTIONS.md
d36ad90 Update LAB.md
59ef18a Update LAB_INSTRUCTIONS.md
37be3c8 Update LAB_INSTRUCTIONS.md
97da547 Update LAB.md
```
- The diagram below shows how the branch created works in relation to the pure lab branch.
  ![Lab Report Branch](./Images/Branch%20Making%20(1).jpg)

# Step 5: Setup a Continuous Integration configuration
- The file is capable of building, testing, and deploying code. The file can be used to specify tasks such as checking code, creating environment variables, and deploy code to production environments. So for the file I selected it runs a hello world statement. The file works through having a workflow which is comprised of jobs which complete various tasks. So in my file there is one job which is say hello and that creates a docker image which is just the config file I selected. Then steps are run which echos hello world that way it can be displayed.


- The first section of the file is jobs which specifies the task that is going to be completed. Next is Say Hello which is the job that is being run and this has a docker section which creates an image of the file itself as it specifies where things are being executed from. From there steps is used to say what needs to get done which is where echo is specified to make the file say hello world. Then at the end the workflow is called which means that the jobs get run. 
   

- When a build is successful at its core it means everything passed the tests that were specified for the code. So the code that was added did not cause any major issues and meet the quality stanards specified for the code. Finally it means that the build is stable enough to move forward in testing or be deployed.
   

- I would add more words to make it say more than just hello world and I would begin trying to figure out if it were possible to add images so that way it would have something nice than just plain text. Also even though the build suceeded it still failed some tests so I would work on trying to see why those tests failed.
   

# Step 6: Merging the feature branch
* The output of my git commit log
```
664b162 (HEAD -> purelab, origin/labreport, labreport) This is the finished product
e661bd1 @trevordbunch
94babae (upstream/purelab, upstream/HEAD, origin/purelab, origin/HEAD) Merge pull request #59 from JeffSinsel/purelab
2e92bd8 Fixed typos and links in markdown files
fa4fc85 Update Instructions
f8513e0 Update Node links to Instructions
d4f22eb Update repo branch names
0e3ae4c Reset purelab
050b420 Merge pull request #2 from trevordbunch/main
1fe415c Merge pull request #1 from trevordbunch/labreport
13e571f Update Lab readme, instructions and templates
eafe253 Adjust submitting instructions
47e83cd Add images to LabReport
ec18770 Add Images
dbf826a Answer Step 4
a9c1de6 Complete Step 1, 2 and 3 of LAB_TREVORDBUNCH
1ead543 remove LAB.md
8c38613 Initial commit of labreport with @tangollama
dabceca Merge pull request #24 from tangollama/circleci
a4096db Create README.md
2f01bf4 Update LAB_INSTRUCTIONS.md
347bd50 Update LAB_INSTRUCTIONS.md
7aaa9f3 Update LAB_INSTRUCTIONS.md
37393ae Bug fixed
1949d2a Update LAB_INSTRUCTIONS.md
d36ad90 Update LAB.md
59ef18a Update LAB_INSTRUCTIONS.md
37be3c8 Update LAB_INSTRUCTIONS.md
97da547 Update LAB.md
0bd6244 updated Step 0 title
4562cd8 added npm and node install repreq
255051e adding template
13a09b7 Adding the LAB.md and correcting some instructions.
d2ddea5 Version 0.0.1 of the lab isntructions
ab312fc more progress
62fb0a5 more progress
fe1937b more in the lab instructions
3e807fb first section
9ae6b83 remove LAB.md
e429c1a lab instructions
ce1fcea circleci default config
80bbdbb circleci default config
968099e remove test db
7362cd1 working
44ce6ae Initial commit
```


![CircleCI Success](./Images/Screenshot%202023-02-06%20011315.png)



