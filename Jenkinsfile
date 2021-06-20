pipeline {
    agent any
    stages {
        stage('git repo'){
            steps{
                bat "rmdir /s /q time-tracker"
                bat "git clone https://github.com/Nirmalrajhen/time-tracker.git"
                bat "mvn clean -f time-tracker"
            }
        }
        stage('test'){
            steps{
                bat "mvn test -f time-tracker"
            }
        }
         stage('build'){
            steps{
                bat "mvn package -f time-tracker"
            }
        }   
    }
}
