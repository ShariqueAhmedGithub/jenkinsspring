pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "MyMaven"
    }

    stages {
        stage('compile') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/sharique16/jenkinsspring.git'
                // Run Maven on a Unix agent.
                sh "mvn compile"
            }
        }
         stage('test') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/sharique16/jenkinsspring.git'
                // Run Maven on a Unix agent.
                sh "mvn test"
            }
        }
         stage('package') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/sharique16/jenkinsspring.git'
                // Run Maven on a Unix agent.
                sh "mvn package"
            }
        }
    }
}
