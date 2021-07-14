pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    
    stages{
        stage('build'){
            steps{
                echo 'this is the BUILD job'
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                echo 'this is the TEST job'
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the PACKAGE job'
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
