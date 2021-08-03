pipeline {
   agent {
           node { label 'jenkins-slave1' 
               
           }
		   
       }
       options { 
	buildDiscarder(logRotator(numToKeepStr: '10'))
		
	}
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage("test"){
           steps{
            echo "test"
        } 
        }
        
    }
}
