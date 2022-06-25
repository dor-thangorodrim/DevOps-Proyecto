pipeline {
    agent any
    tools {
        maven 'M3_8_6'
    }
    stages {
        
        stage('Compile') {
            steps {
                dir('Servicios/Curso-Microservicios') {
                    sh 'docker build -t microservicio .'
                }
            }
        }
        stage('Push Image') {
            steps {
                withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: '', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD']]) {

                }
            }
        }
    }
}