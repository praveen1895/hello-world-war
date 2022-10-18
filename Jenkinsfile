pipeline { 
    agent {label 'slave1'}
    stages { 
        stage ('checkout') { 
            steps {
                sh "pwd"
                sh "rm -rf hello-world-war"
                sh "git clone https://github.com/praveen1895/hello-world-war.git"
            }
        }
        stage ('Test') { 
             steps {
                echo "Testing"
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
