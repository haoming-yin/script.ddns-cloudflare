pipeline {
    agent {
        label "pi"
    }

    stages {
        stage("Demo step") {
            steps {
                sh "printenv | grep 'JENKINS_'"
            }
        }
    }
 
    post {
        always {
            cleanWs()
        }
    }
}