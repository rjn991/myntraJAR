pipeline {
    agent {
        label "java_tech"
    }
    tools {
        maven 'maven'
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage("info") {
            steps {
                sh "pwd"
                sh "uptime"
                sh "whoami"
                echo "$HOSTNAME"
            }
        }
     }
    
}
