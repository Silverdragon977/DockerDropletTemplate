# DockerDropletTemplate
This template is set to work with DigitalOcean 1-click docker droplet. It gets everything going for Setup Scripts, YAML files, and Laravel + React + Typescript Template for easy website creation in the future! 


# User Guide
First click "Use Template" and create a new repo
Next we clone that repo locally
Then we can make a dev branch and setup CI/CD as well as print statements
After that we can go into a DigitalOcean Droplet with 1-click Docker setup from the marketplace
Then we verify the ssh keys with github and clone it to production
We can then use the pullFromGitClean2.sh to pull changes as they happen on main manually or use CI/CD
Lastly we run the setup.sh script which will run the YAML files and helper scripts to setup the environment 


# Development -> Production Cycle

Make changes   ->     push changes to dev     ->      Run automated merge checks and unit testing    ->       Make more changes till end of sprint
   Local                  Github                                       Github                                       Github
                                                                                                                       |
                          ^                                                                                             |
                          |                                                                                             V
                          |                                                                                             
   Make more Changes if sprint isn't over      <-            Merge Dev to Main Successfully          <-          Make sure CI/CD Tests pass 
Else Pull changes to Prod Manually or Auto 

