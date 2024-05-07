pipeline {

  stages {

    stage('Build') {
      steps {
        
        script {
          git branch: 'main', 
             credentialsId: 'GIT_ID', 
             url: 'https://github.com/Arbythecoder/nexa-jenkins.git' 
        }

        sh 'mvn clean package' 

     
        sh 'mvn test' 
      }
    }

  }
}
