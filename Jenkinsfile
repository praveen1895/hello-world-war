pipeline { 
    agent { label 'slave2' } 
    stages { 
        stage ('Checkout') { 
            steps {
                sh "pwd"
                sh "rm -rf hello-world-war"
                sh "git clone https://github.com/praveen1895/hello-world-war.git"
            }
        }
        stage ('Build') { 
             steps {
                sh "ls"
                sh "cd hello-world-war"
                sh "mvn clean package"
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
