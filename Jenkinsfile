pipeline {
    agent any

    stages {
        stage('Run Python') {
            steps {
                sh '''
                echo "Running Python..."
                cd python
                python3 app.py
                '''
            }
        }

        stage('Run Java') {
            steps {
                sh '''
                echo "Running Java..."
                cd java
                javac Hello.java
                java Hello
                '''
            }
        }
    }
}


