pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
        stage('Deploy') { 
            steps {
                sh 'su yum install -y expect'
                sh 'sh /home/lucy/sh/test.sh' 
            }
        }
    }
}
