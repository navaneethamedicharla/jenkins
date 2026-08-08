pipeline {
agent any

tools {
    maven 'maven'
    jdk 'java'
}

stages {
    stage('Build & Test') {
        steps {
            echo 'Jenkins pipeline is working successfully!'
            sh 'java -version'
            sh 'mvn -version'
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
        echo 'Pipeline completed successfully!'
    }
    failure {
        echo 'Build failed. Check logs above.'
    }
}

}
