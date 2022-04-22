# Hosting a fullstack application with AWS

### Application used for this project

- I used Udagram project provided from udacity to apply all I've learned in deployment.
- the url to this projectc is (https://github.com/udacity/nd0067-c4-deployment-process-project-starter)
- Added all scripts needed at front and back packages.json.
- Added all scripts needed at the root package.json to navigate to front and back and execute aforementioned scripts.
- Added screenshots for all AWS services.
- Linked the application parts together (S3, RDS, Elastic beanstalk).
- To access the application use this link (http://udagram-123bucket.s3-website-us-east-1.amazonaws.com)

## Pipeline process inside circle.

### Continuos integration:

- Add the comments needed for installing, testing, building the application at circleci.
- Add the jobs needed to execute the scripts at the root package.json.

### Continuos Delivery/Deployment:

- Link circleci with my github account and access the target project via the config.yml file I previously created with the master branch.
- Added all the environment variables to circleci so it can pass it to the application.
- Added all the applications that we wan to install first to our environment with their version number at "orbs"
- Added the needed "jobs" inside circleci config.yml file to invoke the pre written scripts inside package.json files.
- circleci status badge: [![CircleCI](https://circleci.com/gh/circleci/circleci-docs.svg?style=svg)](https://app.circleci.com/pipelines/github/Islamsulaiman)
- under "workflows" I added a flags to invoke building with circleci only when the main branch has been updated.
