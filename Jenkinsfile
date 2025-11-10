pipeline{
    agent any

    stages{
        stage('Checkout'){
            steps{
                checkout scm
            }
        }

        stage('Validate HTML'){
            steps{
                echo 'validating..'
            }   
        }

        stage('Archive'){
            steps{
                archiveArtifacts artifacts:'register.html',fingerprint:true
            }
        }

        stage('Deploy'){
            steps{
                echo 'Deploying to web server'
            }
        }
    }
}
