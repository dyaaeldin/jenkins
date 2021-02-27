pipeline {
    agent any
    environment {
        ENV1 = "VALUE1"
    }
    stages {
        stage('Build') {
            steps {
                // run your build scripts
                checkout scm
                sh '''
                        echo "Deploying...."                      
                    '''
            }
            // post build section to use "publishBuildRecord" method to publish build record
            post {
                success {
                sh '''
                        echo "Deploying...."                      
                    '''
                }
            }
        }
        stage('Unit Test') {
            steps {
                sh '''
                        echo "Deploying...."                      
                    '''
            }
            // post build section to use "publishTestResult" method to publish test result
        }
        stage('Deploy to Staging') {
            steps {
                sh '''
                        echo "Deploying...."                      
                    '''
            }
        }
        stage('Deploy to dev') {
            steps {
                sh '''
                        echo "Deploying...."                      
                    '''
            }
        }
        stage('Deploy to Prod') {
            steps {
                // Push the Weather App to Bluemix, production space
                sh '''
                        echo "Deploying...."                      
                    '''
            }
            // post build section to use "publishDeployRecord" method to publish deploy record and notify OTC of stage status
            post {
                success {
                sh '''
                        echo "Deploying...."                      
                    '''
                }
                failure {
                sh '''
                        echo "Deploying...."                      
                    '''
                }
            }
        }
    }
}
