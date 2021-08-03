pipeline {
   agent {
           node { label 'jenkins-Slave1' 
               customWorkspace '/var/lib'
           }
		   
       }
       options { 
	buildDiscarder(logRotator(numToKeepStr: '1'))
		retry(3)
		quietPeriod(30)
		timeout(time: 1, unit: 'HOURS')
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
