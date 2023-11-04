pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
               //bat "rmdir  /s /q jenkin-cicd"
                bat "git clone https://github.com/shivamanandb/College-Website.git"
                //bat "mvn clean -f jenkin-cicd"
            }
        }

        stage('checkout') {
            steps {
                bat script:'''
                    xcopy /s /e /y "D:\\Web D assignment\\End sem project\\College Website" "C:\\Apache24\\htdocs"
                ''' 
            }
        }
    }
}
