pipeline {
    agent { label 'Jenkins-Agent'}
    tools {
        jdk 'Java17'
        maven 'Maven3'
    }
    stages {
      stage ("workspace cleanup"){
          steps {
          cleanWs()
              
      }
      }
     stage ("code checkout"){
        steps {
         git branch: 'main', credentialsId: 'github', url: 'https://github.com/Puneet231/jenkinstest'
         

    }
     }
    stage ("build appication"){
        steps {
         sh 'mvn clean package' 
}
            }




    }
}
