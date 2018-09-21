pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
       {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                {
                    sh 'mvn test'
                }
            }
        }


        stage ('Packaging') {
            steps {
                {
                    sh 'mvn clean package'
                }
            }
        }
    }
}
