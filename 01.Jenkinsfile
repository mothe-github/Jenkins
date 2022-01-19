pipeline () {
    agent any
    parameters {
        string(name: 'RETAIL_PROJECT_NAME', defaultValue: '', description: 'Enter the Name of your commercial project')
        choice(name: 'PROJECT_ENV', choices: ['PROD', 'STAGE', 'DEV'], description: 'Pick the environment')
        booleanParam(name: 'FORCE_CREATE', defaultValue: true, description: 'Do you want to create forcefully')
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