pipeline {
    agent any

    stages {
        stage('scm') {
         
            steps {
                 
                    'checkout scm'
                 }
        }
                
        
        stage ('Compile Stage') {

            steps {
                    sh 'mvn clean compile'
                }
            }
        

        stage ('Testing Stage') {

            steps {
                    sh 'mvn test'
                }
            } 
    


        stage ('Deployment Stage') {
            steps {
                
                    sh 'mvn deploy'
                }
            }
        }
    }
