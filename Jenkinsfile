pipeline {
    agent any
environment {

      sonar_url = 'http://localhost:9000/'
      sonar_username = 'admin'
      sonar_password = 'admin'
}
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
                sh 'git clone hhttps://github.com/ashokthummala79/testing-pipeline.git'
            }
        
        }
		stage('Maven') {
            steps {
                sh '''
		cd ${WORKSPACE}/Ashokkumar/Ashokkumar_001/
                mvn clean install -U  -Dmaven.test.skip=true 
		   '''
            }
        
            }
		
	}
}
