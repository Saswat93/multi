pipeline {
    agent any
    
    tools{
        
        maven "M3"
    }
    
    stages {
        
        stage (' Perform GitHub Checkout'){
            steps {
                echo "==============GitHub Checkout Started============="
                git 'https://github.com/Saswat93/java-maven-junit-helloworld.git'
            }
        }
		    stage ('Maven Build Started'){
            steps {
                bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }
        
        }
		}
		}