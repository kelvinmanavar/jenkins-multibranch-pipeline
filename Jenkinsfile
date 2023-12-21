pipeline {
    agent any
    stages{
        stage("Hello"){
            steps {
                echo "Hello Jenkins"
            }
        }
        stage("cat README") {
            when {
                branch "fix-*"
            }
            steps {
                sh 'cat README.md'
            }
        }
    }
}
