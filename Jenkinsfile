pipeline {
    agent any 
    stages {
        stage('-----clean----') { 
            steps {
                sh "git clone  https://github.com/enasareen/my-app.git"
                sh "mvn clean -f my-app"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test"
            }
        }
        stage('---package---') { 
            steps {
                sh "mvn package"
            }
        }
    }
}
