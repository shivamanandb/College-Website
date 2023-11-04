pipeline {
    agent any
    stages {
 stage('Checkout') {
            steps {
                // Check out the code from your GitHub repository
                checkout([$class: 'GitSCM', 
                    branches: [[name: 'main']], 
                    doGenerateSubmoduleConfigurations: false, 
                    extensions: [], 
                    submoduleCfg: [], 
                    userRemoteConfigs: [[url: 'https://github.com/shivamanandb/College-Website.git']]
                ])
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
