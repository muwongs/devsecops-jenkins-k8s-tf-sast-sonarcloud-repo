pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=italebuggywebapp -Dsonar.organization=italebuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=04cc3ca07032bcc6d7c9fe6860c0aa8d357127f3'
			}
        } 
  }
}
