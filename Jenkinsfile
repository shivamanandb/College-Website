pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
               //bat "rmdir  /s /q jenkin-cicd"
                bat "git clone "https://github.com/shivamanandb/College-Website.git"
                //bat "mvn clean -f jenkin-cicd"
            }
        }
        stage('install') {
            steps {
                bat "mvn install -f jenkin-cicd"
            }
        }
        stage('test') {
            steps {
                bat "mvn test -f jenkin-cicd"
            }
        }
        stage('package') {
            steps {
                bat "mvn package -f jenkin-cicd"
            }
        }
    }
}
