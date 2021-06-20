pipeline {
    agent any
    stages {
        stage('git repo'){
            steps{
                bat "git clone https://github.com/Nirmalrajhen/time-tracker.git"
                bat "mvn clean -f time-tracker"
            }
        }
        stage('test'){
            steps{
                bat "mvn test -f time-tracker"
            }
        }
            
    }
}
