## What is continuous integration?

Continuous Integration means developers regularly add their code changes to a shared repository. Whenever new code is pushed, automated builds and tests can run to check if everything is working properly.

## What is continuous delivery?

Continuous Delivery means keeping the application in a state where it can be released at any time. After the code passes the required tests, it is prepared for deployment.

## Circle CI

CircleCI is a continuous integration and delivery platform that can be connected to a GitHub repository.

It can automatically build and test the project whenever changes are pushed to GitHub.

Main uses :

- Automatically build projects
- Run automated tests
- Run CI workflows for different branches

CircleCI uses a configuration file to define the steps that should be executed.
The configuration is commonly stored at: .circleci/config.yml
In this file the steps to be performed for tests are defined.
