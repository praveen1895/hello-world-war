pipeline { 
    agent {label 'slave1'} 
    stages { 
        stage ('checkout') { 
            steps {
                sh "pwd"
                sh "rm -rf hello-world-war"
                sh "https://github.com/praveen1895/hello-world-war.git"
            }
        }
        stage ('build') { 
             steps {
                sh "ls"
                sh "cd hello-world-war"
                sh "mvn clean package"
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
