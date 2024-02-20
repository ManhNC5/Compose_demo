pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=fe-lab-devsecops_lab-devsecop2024 -Dsonar.organization=fe-lab-devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=8a2c0ccbc092a71c19377cb9bc538e9d26189614'
		  }
        } 
  }
}
