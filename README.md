# Unnamed Company DevOps Interview Project
<<<<<<< HEAD
This is a DevOps project I have done while interviewing with a tech company in 2018. I cannot name the company as I signed an non-disclosure letter not to reveal the company name. I have designed and developed a simplified CI/CD for the webapp and explained my solution in the Devops_Design_Document.pdf file.
=======
This is a DevOps project I have done while interviewing with a tech company in 2018. I cannot name the company as I signed an non-disclosure letter not to reveal the company name. 
>>>>>>> 4959d88750e7e87399acf7b4aad9533998eae098

I have designed and developed a simplified CI/CD pipeline for a web application and explained my solution in the Devops_Design_Document.pdf file.

## Original Interview Question (DevOps)

The purpose of this project is to design and implement a CI/CD system for a ToDo web application. You are expected to create a short design document, and to prototype the CI/CD system in a Docker environment.
There is no right-or-wrong answer, but you are expected to deliver a working solution. You can ask questions and seek help if there is anything that you are not familiar with. You should spend about 8-12 hours.

For your convenience, a ZIP file with initial Git repository and a ​docker-compose.yml​ file are provided to get you started.
- Unzip the file and run:
$ docker-compose up -d
- This will start a Git SSH server container and a NGIX server running the application
- Visit ​http://localhost:8082​ to test that the web app is running
- Copy your public SSH key into the ./git-server/keys directory
- To checkout the Webapp sources, run:
$ git clone ssh://git@localhost:2222/git-server/repos/webapp.git
- Note that the WebApp is already checked out under webapp
Project Goals
- Write a short design document that describes the CI/CD system
- Setup a CI pipeline in Jenkins (in a Docker environment) that is:
○ Polling the local Git repository for changes
○ Rebuilds the Docker image when a change is detected
○ Note that the CI/CD scripts should be managed/versioned
- Implement a deployment option that allows a user to Deploy a specific version
○ To deployment a new version, stop the currently running “webapp” container and
start the newly built container
Deliverables
Deliver a ZIP (or tar.gz) file of the project directory that contains all necessary files, similar to the provided bootstrap environment. In particular, provide:
- A PDF design document that describes the CI/CD system
- Document describing your implementation
- Instructions on how to run and test the system

## Solution

Please read the Design Document PDF before executing the docker-compose file.

Remember to copy your public SSH key in the ./git-server/keys directory.
See https://github.com/jkarlosb/git-server-docker for more info on using the Git Server container.

