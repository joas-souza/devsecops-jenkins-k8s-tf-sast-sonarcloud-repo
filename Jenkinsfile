pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=tdsobuggywegapp -Dsonar.organization=tdsobuggywegapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=31c484b7c89ed2207d02e591f97e2fe9a2dac935'
			}
        } 
  }
}
