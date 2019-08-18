
pipeline {
    agent any

    stages {
        stage ('Compile Stage Test ') {

            steps {
                withMaven(maven : 'maven_3_6_1') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage Test') {

            steps {
                withMaven(maven : 'maven_3_6_1') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage Test') {
            steps {
                withMaven(maven : 'maven_3_6_1') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}