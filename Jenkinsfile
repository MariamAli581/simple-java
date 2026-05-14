node {
    // سحب الكود من GitHub
    git branch: 'main', url: 'https://github.com/MariamAli581/simple-java.git'

    stage('Build') {
        try {
            // إضافة مسافة بعد echo وقفل علامة التنصيص صح
            sh 'echo "build stage"'
        } 
        catch (Exception e) {
            sh 'echo "error found"'
        }
    }

    stage('Test') {
        // مراجعة الشرط وقفل الأقواس بشكل سليم
        if (env.BRANCH_NAME == "feat") {
            sh 'echo "test stage"'
        } 
        else {
            sh 'echo "skip"'
        }
    }
}