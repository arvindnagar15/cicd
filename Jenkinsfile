pipeline {

    agent any
    tools {
        maven 'Maven_3.6.1' 
    }
    stages {
        stage('Compile stage') {
            steps {
                bat "mvn clean compile" 
        }
    }

         stage('testing stage') {
             steps {
                bat "mvn test"
        }
    }

          stage('package stage') {
              steps {
                bat "mvn package"
        }
    }
        stage('deployment stage') {
              steps {
                bat "mvn deploy"
        }
    }

  }

}
