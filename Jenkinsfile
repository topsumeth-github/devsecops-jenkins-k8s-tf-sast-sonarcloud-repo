pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=topsumeth-wepapp -Dsonar.organization=topsumeth-wepapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9db76d37cf202a3ff0bbe1631d928b9b9553d776'
			}
        } 
  }
}
