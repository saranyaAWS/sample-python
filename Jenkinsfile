pipeline{
    agent any   
stages{
    stage('github'){
        steps{
            git credentialsId: 'github_app', url: 'https://github.com/saranyaAWS/sample-python.git'
        }
    }
    
    stage('build'){
     steps{
        sh 'python3 --version'
        
     }   
    }
    stage('test'){
        steps{
            echo "welcome to testingteam"
        }
    }
    stage('deploy'){
        steps{
            sh 'python3 app.py'
        }
    }
}    
}
