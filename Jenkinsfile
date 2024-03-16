pipeline{

    agent {
        label 'jenkins-container-agent'
    }

    stages{

        stage('build'){
            steps{
                script{
                    sh 'mvn clean package'
                  sh 'docker build -t java-app .'
                    sh 'docker build -t java-app:test .'

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
