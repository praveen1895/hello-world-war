pipeline { 
    agent { label 'slave1' } 
    stages { 
        stage ('Checkout') { 
            steps {
                sh "pwd"
                
            }
        }
        stage ('Build') { 
             steps {
                echo "praveen"
             }
        }
        stage ('Deploy') { 
             steps {
                echo "QA"
             }
        }
        stage ('Deploy') { 
             steps {
                echo "Deploy"
             }
        }
        stage ('Monitor') { 
             steps {
                echo "Monitor"
             }
        }
 
    }           
 }
