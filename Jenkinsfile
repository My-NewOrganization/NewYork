#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: 'Shivakumar',
    projectUrlStr: 'https://github.com/My-NewOrganization/NewYork.git'],
    pipelineTriggers([
      upstream(
      threshold: 'SUCCESS',
      upstreamProjects: 'https://github.com/My-NewOrganization/Massachusetts.git'
      )
    ])
])

node {
  stage 'build'
  echo 'hello world'
  stage 'test'
  echo 'hello veridic'
  stage 'Deploy'
  echo 'hello Georgia'
 }
