node{

    git branch: 'scripted-jenkins-course', url: 'https://github.com/DinaGamalMahmoud/simple-java-app.git'

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
