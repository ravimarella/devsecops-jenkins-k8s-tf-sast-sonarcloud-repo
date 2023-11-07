pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecuritygurubuggywebap -Dsonar.organization=asecuritygurubuggywebap -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=1d26a394bc72b6df318127817c9f490c451b9660'
			}
        } 
  }
}
