pipeline {
    agent none
    stages {
         stage ('Stage1') {
            agent {label 'master'}
            steps {
                git 'https://github.com/Rohan-designer/Test-1.git'
                sh 'mvn clean install'
            }
       }
      stage ('Stage2') {
          agent {label'Slave089'}
                steps {
                    git 'https://github.com/Rohan-designer/Jenkinsproject2.git'
                    sh 'make'
                }
            }
    }
    
}
