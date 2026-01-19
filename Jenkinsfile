pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo '✅ Jenkins 最小闭环成功！'
                sh 'date'
                sh 'echo "当前目录文件:" && ls -l'
            }
        }
    }
}
