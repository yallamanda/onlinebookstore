pipeline {
    agent any

    stages {
        stage('Code Download') {
            steps {
               git 'https://github.com/yallamanda/onlinebookstore.git'
            }
        }
        
        stage('Code Build') {
            steps {
                sh 'mvn package'
            }
        }
        
        stage('Deploy') {
            steps {
                echo "Deploy the war file into QA Server"
            }
        }
    }
}
