pipeline{
    agent any
    tools{
        maven 'maven'
    }
    stages{
        stage("test"){
            steps{
                sh 'mvn clean test'
            }
        }
        stage("build"){
            steps{
                sh 'mvn clean package'
            }
        }
        } 
    }
