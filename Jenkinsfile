pipeline{
    agent any 
        stages{
            stage("build stage) {
                steps{
                   sh 'mvn clean pacakage'
                }
                post{
                    success {
                        Echo "now archiving the artifacts..."
                        archiveArtifacts artifacts: '**/*.war'
                    }
                }
            }
        }

}
     