pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ikilizabuggywebapp -Dsonar.organization=ikilizabuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b9de06f3f3b61f2963c6eaea489085daedebc603'
			}
        } 
  }
}
