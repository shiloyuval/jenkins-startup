pipeline {
    // triggers {
    //     cron '* * * * *'
    // }
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning stage rd /s /q jenkins-startup'
                sh "cd .. && ls"
                
                echo " && git clone https://github.com/shiloyuval/jenkins-startup.git"
                echo "git clone https://github.com/shiloyuval/jenkins-startup.git"
                echo "C:/Users/user/Documents/Projects/sample && rd /s /q A"
                echo "cd c:\\qa\\bin"
                echo "cd C:/Users/user/Documents/Projects/sample && rd /s /q A"
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