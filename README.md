# Wintext Website Frontend 

## Contents
- [Wintext Website Frontend](#wintext-website-frontend)
  - [Contents](#contents)
  - [Introduction](#introduction)
  - [Tools](#tools)
    - [Built With](#built-with)
      - [](#)
    - [Public Domains](#public-domains)
    - [Server IP](#server-ip)
    - [Recursive Apache Write permission in these folders](#recursive-apache-write-permission-in-these-folders)
    - [Version check](#version-check)
    - [For local Development](#for-local-development)
    - [Deployment](#deployment)
        - [DB Change](#db-change)
      - [Windows server: schedule run + queue run](#windows-server-schedule-run--queue-run)
    - [Docker](#docker)
      - [Docker:](#docker-1)
      - [Network : External Network](#network--external-network)
      - [Access container to container](#access-container-to-container)
      - [Command: docker](#command-docker)
      - [Command: docker  : Services](#command-docker---services)
      - [Browser:](#browser)
      - [Workbench:](#workbench)
  - [GIT commit types](#git-commit-types)

## Introduction




## Tools

### Built With


| Build With | Version | Server Version |
| ---------- | ------- | -------------- |
|            |



#### 
```
sudo chmod 777 -R *


```

### Public Domains

- Production URL
- Development URL

  
### Server IP

	

### Recursive Apache Write permission in these folders

### Version check

```
```

### For local Development
```
   
```



### Deployment
```

```







##### DB Change

**script user**
```

```

**DB Permission : Delete**

**Tables:**
- failed_jobs
- jobs

#### Windows server: schedule run + queue run
```
where php
```


### Docker
#### Docker: 

#### Network : External Network
```
sudo docker network create queue_management_network
sudo docker network create local_central_db_network
sudo docker network create local_central_rabbitmq_network


docker exec -it wintext-website-frontend-container sh
```

#### Access container to container
```
docker exec ms-rmq-container ping 103.134.89.185

docker exec ms-rmq-container ping queuemanagement-service-container

docker exec queuemanagement-service-container ping ms-rmq-container 
docker exec queuemanagement-service-container telnet ms-rmq-container 5673
docker exec queuemanagement-service-container ping otl-erp-db-container 
```




#### Command: docker 
```
sudo docker-compose down
sudo docker-compose build && docker-compose up -d
```

#### Command: docker  : Services
```
```

#### Browser: 
- browser: http://localhost:86

#### Workbench:
```

``` 






## GIT commit types
```
feat: New feature for the user.
fix: Bug fix.
style: Code Style Changes.
refactor: Code Refactoring.
build: Build System Changes.
ci: Continuous Integration Changes.
perf: Performance Improvements.
revert: Revert a Previous Commit.
docs: Documentation changes.
test: Adding or modifying tests.
chore: Routine tasks, maintenance, or housekeeping.
```

