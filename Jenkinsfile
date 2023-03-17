pipeline {
    agent any

    stages {
        stage('Dev') {
            steps {
                echo 'tomcatStage'
                build quietPeriod: 5, job: 'tomcat-docker'
            }
        }
        stage('Test') {
            steps {
                echo 'Test-stage'
                build quietPeriod: 5, job: 'tomcat-linux'
            }
        }
       
    }
}
