pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs'nodejs' 
    }
    

    stages{
        stage('Build'){
            steps{
                echo 'this is the Build job'
                sh 'npm intall'
                
            }
        }
        stage('Test'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
                
            }
        }
        stage('Package'){
            steps{
                echo 'this is the package job'
                sh 'npm run package'
                
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
