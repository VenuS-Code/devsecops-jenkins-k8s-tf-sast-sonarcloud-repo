pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=vrbuggywebapp -Dsonar.organization=vrbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=58e63632d3c40db7cad199a55f2c63e0d27571ea'
			}
        } 
  }
}
