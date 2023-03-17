# docker-atlassian-sandbox

Docker compose script created in order to easily create docker containers with the following atlassian products:
* Jira
* Confluence
* Bitbucket

Each container gets its own Postgress Database, that each application is dependent on.

# Usage
You can start up all 3 applications by writing:
```
docker-compose up -d
```
You can also start up single applications by specifying the application afterwards:
```
docker-compose up -d confluence
```

If you want to stop all applications, you can write:
```
docker-compose down
```
# To access Atlassian applications
Applications can be reached by localhost:
```
localhost:8080 (Jira)
localhost:8090 (Confluence)
localhost:7990 (Bitbucket)
```
These can be changed in the file if multiple versions are intended to be run at the same time.

# Directory Structure
```
.
├── bitbucket # data directory for bitbucket
├── bitbucket_pgdata # data directory for bitbucket postgresql database
├── confluence # data directory for confluence
├── confluence_pgdata # data directory for confluence postgresql database
├── docker-compose.yml # docker-compose file
├── jira # data directory for jira
├── jira_pgdata # data directory for jira postgresql database
└── README.md # this file
```
