pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                script{
                    sh 'docker build -t java-app .'
                    sh 'docker build -t java-app:test .'

                }
            }
        }


    stage('build'){
        try{
            sh 'echo "build jenkins scripted pipeline"'
        }
        catch(Exception e){
            sh 'echo "exception found"'
            throw e
        }
    }
    stage ('test'){
        sh 'ech "test failed"'
    }
}
