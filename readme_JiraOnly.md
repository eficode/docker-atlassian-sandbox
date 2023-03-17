# **Jira in docker running on M1 chip**

This is a much easier method to run jira in docker using Apple M1 chip

Running jira using this code was at least 100% faster than JiraArm

# How to use?

* run this command `docker-compose up jira`

* Done!

# How do i access jira?

From your favorite browser go to http://localhost:8080

# How can i change the jira version? 

You can change the jira version in the _Docker compose_ by setting the variable `jiraVersion` to any supported jira version.

The list of all jira versions are available [here](https://marketplace.atlassian.com/apps/1213607/jira-software/version-history)


# What is the difference between this and JiraArm?
In this module you can set the jira version to *ANY* version and it will work using Java 11 . It's also **much faster** and truly uses the power of an M1 chip processor.

## How to setup the database container with postgres? 
Enter the container id of the postgres container

example `Hostname:4ddf08774e41`

You can lookup the container id using `docker ps` command in terminal

add the username and password from the docker-compose file (by default it's jira and jira)

# How to kill and remove all data ? 
by running `docker-compose down -v --rmi all`


## go bananas!


