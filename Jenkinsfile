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
                sh 'sh test.sh' 
            }
        }
    }
}
