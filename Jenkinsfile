pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo '📥 拉取代码...'
                sh 'ls -l'
            }
        }
        stage('Build C Program') {
            steps {
                echo '🔨 编译 C 程序...'
                sh 'gcc main.c -o app'   // 注意：用 gcc 而不是 g++（C 语言）
                sh 'ls -l app'           // 验证可执行文件生成
            }
        }
        stage('Run') {
            steps {
                echo '🚀 运行程序...'
                sh './app'
            }
        }
    }
}
