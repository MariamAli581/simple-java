node{
    git branch: 'main' , url: 'https://github.com/MariamAli581/simple-java.git'
    stage('buld'){
        try{
        sh 'echo"build stage"
        catch(Exeption e){
            sh'echo "found"
        }
        }
    stage('test'){
        if (env.BRANCH_NAME=="feat"){
            sh'echo "test stage"
        
        }
        else{
            sh'echo "skip"
            }
    }
}
