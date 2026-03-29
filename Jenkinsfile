pipeline{
    tools{
        maven 'mymaven'
    }
    agent any // any = any available server where jenkisn can run the pipleine
    
    stages{
        stage('Checkout Code'){
            steps{
               git 'https://github.com/pratikbagade/DevOpsCodeDemo.git'
            }
        }
        stage('Compile Code'){
            steps{
                sh 'mvn compile'
            }
        }
       stage('Review Code'){
            steps{
                sh 'mvn pmd:pmd'
            }
           
        }
    }
}

