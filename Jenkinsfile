pipeline{
    agent any 
        stages{
            stage("build stage") {
                steps{
                   sh 'clean pacakage'
                }
                post{
                    success {
                        echo "now archiving the artifacts..."
                        archiveArtifacts artifacts: '**/*.war'
                    }
                }
            }
        }

}
     