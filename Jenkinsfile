pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('Build'){
            steps{
                echo 'this is the build job'
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                echo 'this is the second job'
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the third job'
                sh 'npm run package'
                sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed for shopping-potal app...'
        }
        
    }
    
}
