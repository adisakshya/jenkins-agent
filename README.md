# Jenkins Agent

**Build great things at any scale**

[![Dockerhub](https://img.shields.io/badge/Dockerhub-blue.svg?style=for-the-badge&logo=appveyor)](https://hub.docker.com/r/adisakshya/jenkins-agent) [![version](https://img.shields.io/badge/Version-1.0.0-blue.svg?style=for-the-badge&logo=appveyor)](https://github.com/adisakshya/jenkins-agent) [![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-blue.svg?style=for-the-badge&logo=appveyor)](https://github.com/adisakshya/jenkins-agent/pulls) [![Open Source](https://img.shields.io/badge/Open%20Source-Love-red.svg?style=for-the-badge&logo=appveyor)]()


Jenkins is a leading open source automation server, it provides hundreds of plugins to support building, deploying and automating any project.

As an organization matures from a continuous delivery standpoint, its building-deploying and automating requirements will similarly grow. 
Jenkins supports the "master/agent" mode, to support distributed build environment, where the workload of building projects are delegated to multiple agents.

This repository contains docker image of a Jenkins agent, which can be used in a distributed build architecture.

An agent is a machine set up to offload projects from the master. The method with which builds are scheduled depends on the configuration given to each project. For example, some projects may be configured to "restrict where this project is run" which ties the project to a specific agent or set of labeled agents. Other projects which omit this configuration will select an agent from the available pool in Jenkins.

## Operating Instructions

### Prerequisites

- Make sure you have
  - Docker installed

### Fork

- Fork this repository
	- "Forking" adds a copy of [adisakshya/jenkins-agent](https://github.com/adisakshya/jenkins-agent/) repository to your GitHub account as `https://github.com/YourGitHubUserName/jenkins-agent`
- Download or clone your forked repository
	- You can clone the repository executing below command in a location of your choice of your system.
	```$ git clone https://github.com/YourGitHubUserName/jenkins-agent.git```

### Using Docker

- Make sure you have docker installed before proceeding.
    - From project-root-directory, run the following command
		- ```docker build -t my-jenkins-agent .```
    - Or you can directly pull the docker image, using following command
    	- ```docker pull adisakshya/jenkins-agent```
- As soon as the build completes you are all set to get started with jenkins-agent.
- Now you can run the docker image using the following command
    - ```docker run -d --name jenkins-agent my-jenkins-agent```

## Suggest Features

Is a feature you care about currently missing? Make sure to browse the [issue tracker](https://github.com/adisakshya/jenkins-agent/issues?q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc) and add your ":+1:" reaction to the issues you care most about, as I also use those reactions to prioritize issues.

## JustStarIt

🌟 Star this repo if jenkins-agent helped you.

## License

All versions of the app are open-sourced, read more about this [LICENSE](https://github.com/adisakshya/jenkins-agent/blob/master/LICENSE).