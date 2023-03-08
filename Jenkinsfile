pipeline {
    agent any
environment {
        DISABLE_AUTH = 'true'
        DB_ENGINE    = 'sqlite'
    }
    stages {
        stage('git repo & clean') {
            steps {
               sh "echo $DB_ENGINE"
            }
        }
    }
}
