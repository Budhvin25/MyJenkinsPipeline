pipeline {
    agent any
    
    triggers {
        pollSCM('H/2 * * * *')  // Check every 2 minutes
    }
    
    stages {
        stage('Build') {
            steps { 
                echo '✅ Building code with Maven' 
            }
        }
        stage('Unit and Integration Tests') {
            steps { 
                echo '✅ Running tests with Jest' 
            }
        }
        stage('Code Analysis') {
            steps { 
                echo '✅ Checking code quality with SonarQube' 
            }
        }
        stage('Security Scan') {
            steps { 
                echo '✅ Scanning for bad guys with Snyk' 
            }
        }
        stage('Deploy to Staging') {
            steps { 
                echo '✅ Sending to test server' 
            }
        }
        stage('Integration Tests on Staging') {
            steps { 
                echo '✅ Testing on test server' 
            }
        }
        stage('Deploy to Production') {
            steps { 
                echo '✅ Sending to real website' 
            }
        }
    }
}
