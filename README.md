# DataLake

This repository hosts our datalake implementation

This repository is a showcase of newly joined service/repo which has 
no awareness of Service360 platform and it does not use any of extended
capabilities (passport, plantuml, API, docs) 

## Dev environment

To setup dev environment simply run

    docker-compose up
    
## Deployment

Deployment to production environment is done by CircleCI and is triggered
by git tag creation.

Staging environment is deployed on every tag creation or push to master/release
branch.

In case you need to manually deploy for whatever reason use following command:

    AWS_PROFILE=... ENV=... VERSION=... make deploy