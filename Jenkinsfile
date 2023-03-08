pipeline {
    parameters {
      choice choices: ['insure-base-docker/insure-base', 'insure-ide/insure-sd', 'insure-ide/insure-ansible','insure-ide/ansible-test-vini'], description: 'Auf welche repository sollte die Tag erstellt?', name: 'GIT_PROJECT'
      string defaultValue: '21.x.x', description: 'Version die als branch oder Tag ersellt werden muss', name: 'GIT_BRANCH', trim: false
    }

    agent any

    stages {
        stage('Cloning Git repository') {
            steps {
               sh "${GIT_BRANCH}"
            }
        }
    }
}
