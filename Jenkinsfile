pipeline {
    agent any

    stages {
      stage('build') {
        steps {
          withMaven(maven: 'Maven3') {
		sh 'mvn clean install'
	  }
        }
      }

     stage('test') {
       steps {
         echo 'Testing...'
       }
     }

  stage('deploy') {
    steps {
      echo 'Deploying...'
      echo 'Done'
    }
  }

 }
}



