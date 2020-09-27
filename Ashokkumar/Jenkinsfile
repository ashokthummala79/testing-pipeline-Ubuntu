pipeline {
    agent any
    stages {
		stage('Build from Maven ROOT')
			{
			steps {
			echo "building root POM from maven project"
			bat 'C:/ProgramFiles/apache-maven-3.6.0-bin/apache-maven-3.6.0/bin/mvn -f Ashokkumar/Ashokkumar_ROOT/pom.xml clean install'
				}
			}
}
}