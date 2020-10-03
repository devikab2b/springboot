pipeline {
    agent any
 parameters {
        separator(name: "BUILD_ENVIRONMENT", sectionHeader: "Build Environment")
        string(defaultValue: "123", description: 'What environment?', name: 'userFlag')
        choice(choices: ['US-EAST-1', 'US-WEST-2'], description: 'What AWS region?', name: 'qa-action')
        text(name: 'DEPLOY_TEXT2', defaultValue: 'One\nTwo\nThree\n', description: 'test')
        
    }
    
    

  stages {
        stage('Build') {
          
          echo 'hello'
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
        stage('test3') {
            if (params.region == 'master') {
                echo 'I only execute on the master branch'
            } else {
                echo 'I execute elsewhere'
            }                        
        }      
    }
}