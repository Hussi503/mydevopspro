pipeline
  agent any {
      tools {
            maven "Maven 3.6.3"
            }
      stages {
              stage('git clone') {
              steps              {
                  git branch: 'main', credentialsId: '44a23619-bf4f-4c82-b779-2d11ee265787', url: 'https://github.com/Hussi503/mydevopspro.git'
                                 }
                                 }          
    stage('maven clean') {
                         sh 'mvn clean'
                         }
    stage('maven compile') {
                              sh 'mvn compile'
                           }
    stage('maven validate') {
                              sh 'mvn validate'
                             }
    stage('maven test') {
                          sh 'mvn test'
                         }
    stage('maven package') {
                         sh 'mvn package'
                            }
}  
  }

