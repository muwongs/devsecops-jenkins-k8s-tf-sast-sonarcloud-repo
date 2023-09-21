pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=italebuggywebap -Dsonar.organization=italebuggywebap -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=18dfe38a5f25c66ad2bc111e27e63fbe703d8756'
			}
        } 
  }
}
