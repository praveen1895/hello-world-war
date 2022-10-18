pipeline { 
    agent {label 'slave1'} 
    stages { 
        stage ('checkout') { 
            steps {
                sh "pwd"
            }
        }
        stage ('build') { 
             steps {
               echo "praveen"
             }
        }
        stage ('QA') { 
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
