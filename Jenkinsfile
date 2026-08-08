```groovy
pipeline {
    agent any

    tools {
        maven 'maven'
        jdk 'java'
    }

    stages {
        stage('Build & Test') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Deploy (Optional)') {
            steps {
                echo 'Deployment stage (add steps if needed)'
            }
        }
    }

    post {
        success {
            echo '✅ Pipeline completed successfully!'
        }
        failure {
            echo '❌ Build failed. Check logs above.'
        }
    }
}
```
