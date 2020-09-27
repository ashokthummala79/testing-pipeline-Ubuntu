pipeline {
    agent any

tools {
        jdk 'Java8'
        maven 'Maven-3.3.9'

      }

    stages {
        stage ('Cleanup the Workspace') {
           steps {
            cleanWs()
          }
        }
		stage('GIT') {
            
	       steps {
                sh 'git clone https://github.com/ashokthummala79/testing-pipeline-Ubuntu.git'
            }
        
        }
		stage('Maven') {
            steps {
                sh '''
		cd ${WORKSPACE}/Ashokkumar/Ashokkumar_ROOT/
                mvn clean install
                   '''
            }
        
            }
		
	}
}
