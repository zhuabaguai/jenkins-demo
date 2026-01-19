pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo '拉取代码...'
                sh 'ls -l'
            }
        }
        stage('Build C Program') {
            steps {
                echo '编译 C 程序...'
                sh 'gcc main.c -o app'   
                sh 'ls -l app'          
            }
        }
        stage('Run') {
            steps {
                echo '运行程序...'
                sh './app'
            }
        }
    }
}
