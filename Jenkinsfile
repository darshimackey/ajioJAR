pipeline{
    agent {
        label 'java_slave_node'
    }
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
        stage("info"){
            steps{
                sh 'pwd'
               sh 'whoami'
                echo $HOSTNAME
        } 
    }
    }
}
