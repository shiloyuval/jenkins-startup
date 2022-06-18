pipeline {
    // triggers {
    //     cron '* * * * *'
    // }
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning stage rd /s /q jenkins-startup'
                cmd "cd C:/Users/user/Documents/Projects/sample && rd /s /q A"
                echo "cd C:/Users/user/Documents/Projects/sample && git clone https://github.com/shiloyuval/jenkins-startup.git"
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