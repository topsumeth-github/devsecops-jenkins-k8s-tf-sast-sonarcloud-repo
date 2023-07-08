pipeline {
  agent any
  tools { 
        maven 'Maven_3_0_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=topsumethwebapp -Dsonar.organization=topsumethwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=d7edfd80bef8e61d8d87cd36beaa7ee330a38510'
			}
        } 
  }
}
