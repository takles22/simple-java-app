pipeline{

    agent {
        label 'jenkins-container-agent'
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

                    echo "test stage"
                }
            }
        }

        stage ('post build stage'){
            steps{
                script{
                    slackSend channel: '#ci-builds', message: 'pipeline success'
                }
            }
        }
    }
}
