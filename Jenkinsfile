pipeline {
    agent any

    stages {
        stage('Dev') {
            steps {
                echo 'Hello-Dev-Stage'
                build quietPeriod: 5, job: 'Tomcat-linux'
            }
        }
        stage('Test') {
            steps {
                echo 'Hello Test-stage'
                build quietPeriod: 5, job: 'tomcat-aws'
            }
        }
        stage('Prod') {
            steps {
                echo 'Hello Prod-stage'
                build quietPeriod: 5, job: 'Tomcat-docker'
            }
        }
    }
}
