pipeline {
     agent any

     stages {
        stages('Build') {
            steps {

                bat "mvn compile"
                bat "mvn clean package"


            }
            post {
                 success {
                      archiveArtifacts 'target/*.jar'

                 }


            }


        }


     }


}
