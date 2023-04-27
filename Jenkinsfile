pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'maven' 
    }
    

    stages{
        stage('Build'){
            steps{
                echo 'this is the Build job'
                sh 'mvn install'
            }
        }
        stage('Test'){
            steps{
                echo 'this is the test job'
                sh 'mvn test'
            }
        }
        stage('Package'){
            steps{
                echo 'this is the package job'
                sh 'mvn package'
            }
        }
    }
    
    post{
        always{
            echo 'Shhoping Carts pipeline completed...'
        }
        
    }
    
}

