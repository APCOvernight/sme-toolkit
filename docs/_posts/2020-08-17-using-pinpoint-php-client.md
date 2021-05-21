---
title:  "Using the PinPoint php Client"
published: true
author: Mike Hingley
categories:
  - tutorials
tags:
  - php
  - tutorial
---
In this walkthrough we will create a simple php script to demonstrate how to integrate your php application with the APC Overnight PinPoint API (PPAPI) Services from APC Overnight.

## To complete this tutorial you will need :
1. A set of credentials for PPAPI
2. Docker Desktop or:
3. PHP version 7 or above with composer installed

Here is the [example code we're going to be using](https://github.com/APCOvernight/pinpoint-client-php-example)

## Installation instructions - Docker
With Docker installed, clone the repository into a known folder. 

```shell
git clone git@github.com:APCOvernight/pinpoint-client-php-example.git
```
now you can execute your DockerFile to stand up a CLI Server which will allow you to test the command.

## What's in the repository
The repository does have a [wiki](https://github.com/APCOvernight/pinpoint-client-php-example/wiki) which is being updated discussing what the application does.

|File|Purpose|
|----|-------|
|header.ans|ANSII Text file for producing the PinPoint Logo within the CLI|
|.gitgnore|Instructs git to ignore the /vendor/ folder.|
|README.md|The readme file for this test project|
|composer.json| The project settings, including the required dependancies|
|composer.lock| The exact versions and hashes of dependancies that have been used in this project|

## Installing your dependancies