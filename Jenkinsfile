pipeline {
    agent any
 parameters {
        string( description: 'What environment?')
        choice(choices: ['US-EAST-1', 'US-WEST-2'], description: 'What AWS region?', name: 'region')
        text(name: 'DEPLOY_TEXT', defaultValue: 'One\nTwo\nThree\n', description: '')
        
    }
  stages {
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