# java-cli-maven-mysql-flyway-simple

## Description
Creates a small database table
called `dog`. All output normally
seen in a terminal will be in `java-srv/log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

Uses flyway migration tool to augment
the schema.

## Tech stack
- java
- maven
  - flyway
  - log4j
  - mysql driver

## Docker stack
- maven:3-openjdk-17
- mariadb:latest

## To run
`sudo ./install.sh -u`
Creates java-srv/log

## To stop
`sudo ./install.sh -d`
Removes java-srv/log

## For help
`sudo ./install.sh -h`

## Credit
- [Java code based on](https://github.com/htorun/dbtableprinter)
- [Flyway serviced based on](https://www.baeldung.com/database-migrations-with-flyway)
