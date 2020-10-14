This project is an example of how to add SonarQube quality gates to
a Jenkins build using the SonarQube Scanner Jenkins plugin.

For a full walkthrough, see the [accompanying article](https://tomgregory.com/sonarqube-quality-gates-in-jenkins-build-pipeline).

## Running

Ensure you have a local installation of Docker.

Run `docker-compose up -d --build` and you'll have access to:

* Jenkins at http://localhost:8080
* SonarQube at http://localhost:9000

## Configuration

Jenkins comes pre-configured, but you'll need to configure SonarQube
as described in the article *[Add SonarQube quality gates to your Jenkins builds](https://tomgregory.com/sonarqube-quality-gates-in-jenkins-build-pipeline#configure-sonarqube)*.

## Usage

Once that's setup, try running the two pipeline jobs:

1. A job that runs against a codebase with good code (expect to pass)
1. A job that runs against a codebase with bad code (expect to fail)