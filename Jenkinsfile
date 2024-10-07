
pipeline {
    agent {
            node {
                label 'maven'
            }
    }

environment{
    PATH = "/opt/apache-maven-3.9.9/bin:$PATH" 
    // this is the path to specify where maven is located else cleandeply will not execute
}
    stages{
        Stage('build'){
            steps{
                sh 'mvn clean deploy'
            }
        }
    } 
}
