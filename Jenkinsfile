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
                sh 'su'
                sh 'yum install -y expect'
                sh 'sh /home/lucy/sh/test1.sh'
                sh '/home/lucy/sh/test.sh' 
            }
        }
    }
}
