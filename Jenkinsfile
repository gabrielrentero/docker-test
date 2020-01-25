pipeline {
    agent jenkins
    stages {
        stage('test') {
            steps {
                script {
                    app = docker.build("test/other")
                    app.inside {
                        sh 'echo hello-test'
                    }
                }
            }
        }
    }
}
