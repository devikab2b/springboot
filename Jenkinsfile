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
           if(params.qa-action == 'US_EAST_1') {
       echo 'hello2'
       steps {
                
                         echo 'Building..'
                                           
                

               
            }
       
    } else {
          
          echo 'hello'
          steps {
                
                         echo 'Building..'
                                           
                

               
            }
          
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