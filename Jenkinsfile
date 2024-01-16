pipeline
{
    
    agent any
    
    tools{
    maven 'maven'
    }
    
    stages{
        
        stage("Build"){
            steps{
                git 'https://github.com/jglick/simple-maven-project-with-tests.git'
                sh "mvn -Dmaven.test.failure.ignore=true clean package"
            }
        }
        
        stage("Run UTs"){
            steps{
                echo("Run unit tests")
            }
        }
        
        stage("Deploy to Dev"){
            steps{
                echo("Deploying to Dev environment")
            }
        }
        
        
    }
    
    
}