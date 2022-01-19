pipeline () {
    agent {
        label 'JAVA_AGENT'
    }
    stages {
        stage ('download Jenkinsfile from git') {
            steps {
                git branch: 'main', url: 'https://github.com/mothe-github/Jenkins.git'
            }
        }
        stage ('uptime') {
            steps {
                sh 'uptime'
            }
        }
    }
}