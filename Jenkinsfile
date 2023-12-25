pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devopsudemycourse_dev-test -Dsonar.organization=devopsUdemyCourse -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=5662f9b801f7de2aba3b873a203ca5d20f02f98e'
			}
        } 
  }
}
