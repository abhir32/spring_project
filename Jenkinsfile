pipeline{
    agent any 
    {
        stages{
            stage({
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
     