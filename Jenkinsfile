pipeline {
    agent none
    stages {
        stage ('Clean and Make') {
            parallel {
         stage ('Clean') {
            agent {label 'master'}
            steps {
                git 'https://github.com/Rohan-designer/Test-1.git'
                sh 'mvn clean install'
            }
       }
      stage ('Make') {
          agent {label'Slave089'}
                steps {
                    git 'https://github.com/Rohan-designer/Jenkinsproject2.git'
                    sh 'make'
                }
            }
    }
    
}
    }
