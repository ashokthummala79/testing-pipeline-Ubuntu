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
<<<<<<< HEAD:Jenkinsfile
                sh 'git clone hhttps://github.com/ashokthummala79/testing-pipeline.git'
=======
                sh 'git clone https://github.com/ashokthummala79/testing-pipeline.git'
>>>>>>> b65c158740d6e2b0cfc355873e75a7640625768a:Jenkinsfile.txt
            }
        
        }
		stage('Maven') {
            steps {
                sh '''
<<<<<<< HEAD:Jenkinsfile
		cd ${WORKSPACE}/Mounika/Mounika_001/
=======
				cd ${WORKSPACE}/Rajyalakshmi
>>>>>>> b65c158740d6e2b0cfc355873e75a7640625768a:Jenkinsfile.txt
                mvn clean install -U  -Dmaven.test.skip=true 
		   '''
            }
        
            }
		
	}
}
