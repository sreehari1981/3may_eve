#!/usr/bin/env groovy
import java.net.URL

node{
    stage('Git checkedout'){
        git 'https://github.com/edureka-git/DevOpsClassCodes.git'
    }
    stage('Project Compile'){
        withMaven(maven:'MyMaven'){
            sh 'mvn compile'
        }
    }
     stage('Project Package'){
        withMaven(maven:'MyMaven'){
            sh 'mvn package'
        }
    }
}
