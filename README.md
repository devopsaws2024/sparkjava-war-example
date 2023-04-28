# sparkjava-war-example
Build war with maven and sparkjava framework

Steps:

1. Download a fresh [Tomcat 8 distribution](https://tomcat.apache.org/download-80.cgi)
2. Clone this repository to your local machine
3. Run mvn package
4. Copy the generated `sparkjava-hello-world-1.0.war` to the Tomcat `webapps` folder
5. Start Tomcat by running `bin\startup.bat` (or `bin\startaup.sh` for Linux)
5. Tomcat will automatically deploy the war
6. Open [http://localhost:8080/sparkjava-hello-world-1.0/hello](http://localhost:8080/sparkjava-hello-world-1.0/hello) in your browser
7. Stash: Stash is used for storing the changes in temporary location.
       
Scenario :  Lets suppose,we are working in one branch(login-feature), edit few files and added files to staging area.
            Now suddenly , we got new hotfix - live/production env , its emergency to fix in next 1 hour.
            But Git best practices says, either you commit your changes or undo the changes back.
            We want to store changes in temporary location  ie your stash concept in git.

commands : git stash list  //list all stashes
           git stash save "some messages"  // creating an stash
           git stash show stash_name  //describe the stash changes
           git stash apply  // It will bring the stash changes out and also will keep one copy of stash entry in stash location.
           git stash pop  // It will bring the stash changes out but it will delete the stash entry from  stash location
           git stash drop  // it will remove all entries from stash
