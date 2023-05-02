pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
	    	sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ass2key -Dsonar.organization=ass2key -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f561e00d0ee7742bcd8bd5365f37913660534aed'
			}
        } 
  }
}
