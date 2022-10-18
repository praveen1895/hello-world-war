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
        stage ('build') { 
             steps {
                sh "ls"
                sh "cd hello-world-war"
                sh "mvn clean package"
             }
        }
        stage ('deploy') { 
             steps {
                 sh "rm -rf hello-world-war-1.0.0 hello-world-war-1.0.0.war"
                sh "cp /home/slave1/workspace/pipelinejob1/target/hello-world-war-1.0.0.war /opt/tomcat/webapps"
                 sh "sudo systemctl restart tomcat.service"
             }
        }
        stage ('QA') { 
             steps {
                echo "QA"
             }
        }
        stage ('Monitor') { 
             steps {
                echo "Monitor"
             }
        }
 
    }           
 }
