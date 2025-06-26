pipeline {
    agent {
        docker {
            image 'mcr.microsoft.com/dotnet/sdk:8.0'
            args '-u root:root'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'dotnet --version'
                sh 'dotnet restore'
            }
        }
    }
}
