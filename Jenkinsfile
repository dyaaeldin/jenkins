pipeline{
    agent any
    environment {
        NEW_ENV = '1.3.5'
    }
    stages{
        stage('build'){
            steps{
                echo "building"
            }
        }
        stage('test'){
            steps{
                echo "testing"
            }
        }
        stage('deploy'){
            steps{
            //    withCredintials([
              //      usernamePassword(credintials: 'id1', usernameVariables: USER1 , passwordVariable: PASS1)
                    // this will use cred with id1 and define variable USER1 with value of username in credintial stored in jenkins
                // ]) {
                  //  sh "ssh ${USER1}@ip uptime"
			echo "deploy"
                }
            }
        }
        post{
            always{
                echo "done"
            }
        }
    }
}
