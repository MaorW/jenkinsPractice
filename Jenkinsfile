"""
Write a pipeline script that run 4 stages:
fetching -> echo fetching
building -> echo building
testing -> echo testing
deploying -> echo deploying

Upload the file to a new repo in your github using git commands

"""
pipeline{
    agent any
    stages{
        stage("fetching"){
            steps{
                echo "========fetching========"
            }
            
        }
        stage("building"){ // Should be under timeout
            steps{
                echo "========building========"
            }
            
        }
        stage("testing"){
            steps{
                echo "========testing========"
            }
            
        }

        stage("deploying"){ // Should be under timeout
            steps{
                echo "========deploying========"
            }
            
        }
        
    }
    post{
        always{ // Should be used for closing connections.. files.. Containers..
            echo "====++++always++++===="
        }
        success{ 
            echo "====++++only when successful++++===="
        }
        failure{
            echo "====++++only when failed++++===="
        }
    }

   
}