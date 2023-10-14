node{
    git branch: 'scripted-pipeline', url: 'https://github.com/DinaGamalMahmoud/simple-java-app.git'
    stage('build'){
        sh 'echo "build stage"'
        try{
            if ( env.BRANCH_NAME == 'scripted-pipeline' ){
                sh 'echo "we are in build stage"'
            }
        }catch(Exception e){
            throw e
        }
    }
    stage('test'){
        sh 'echo "test stage"'
    }
}
