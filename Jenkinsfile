pipeline { 
    agent {label 'slave1'} 
    stages { 
        stage ('checkout') { 
            steps {
                sh "pwd"
                sh gitclone "git clone https://github.com/praveen1895/hello-world-war.git"
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
