pipeline {
    agent any

    stages {
        stage('Vaidation') {
            steps {
                echo 'Validate Project..'
		 sh 'mvn validate'
		 sh 'mvn compile'
            }
        }
        stage('UnitTest') {
            steps {
                echo 'Testing..'
		sh 'mvn test'
	
            }
        }
              stage('Package') {
            steps {
                echo 'build..'
		sh 'mvn package'
            }
        
        }
          
    }
}
