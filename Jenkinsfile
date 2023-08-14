pipeline{
    agent any 
        stages{
            stage("build stage") {
                steps{
                   sh 'mvn clean pacakage'
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
     