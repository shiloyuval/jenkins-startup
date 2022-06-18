pipeline {
    // triggers {
    //     cron '* * * * *'
    // }
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning stage'
                cmd "cd C:/Users/user/Documents/Projects/sample"
                cmd "rd /s jenkins-startup"
                cmd "git clone https://github.com/shiloyuval/jenkins-startup.git"
            }
        }

        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}