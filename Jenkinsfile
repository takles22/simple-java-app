node{

    git branch: 'scripted-jenkins-course', url: 'https://github.com/DinaGamalMahmoud/simple-java-app.git'

    stage('build'){
        try{
            sh 'echo "build stage"'
        }
        catch(Exception e){
            sh 'echo "exception found"'
            throw e
        }
    }
}
