pipeline {
  agent any
  tools { 
        maven 'Maven_3_0_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=topsumethwebapp -Dsonar.organization=topsumethwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b44d74eac5283cb402b29940e428dea169090ddc'
			}
        } 
  }
}
