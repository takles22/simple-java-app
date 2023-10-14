pipeline{
    agent {
    label 'jenkins-mvn-agent'
    }
    stages{
        stage('build'){
            steps{
                script{
                   sh 'mvn clean package'
                }
            }
        }

        stage('test'){
            steps{
                script{
                    sh 'mvn test'

                }
            }
        }
    }
}