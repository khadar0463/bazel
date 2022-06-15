pipeline {
    agent any
    stages {
        stage ('Checkout') {
            steps{
                Checkout scm
            }
        }
        stage('Bazel build') {
            steps {
                sh "cd /var/lib/jenkins/workspace/bazel/examples/cpp;bazel build hello-world"
            }
        }
    }
}
