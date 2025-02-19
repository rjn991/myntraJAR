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
                pwd
                uptime
                whoami
                echo "$HOSTNAME"
            }
        }
     }
    
}
