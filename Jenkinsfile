pipeline {
    agent any
    stages {
        stage ("Build") {
            steps {
                sh 'env -DskipTests clean package'
            }
        }
        stage ("Test") {
            steps {
                sh 'mvn test'
            }
        }
    }
}
