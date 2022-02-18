pipeline {
    agent any

    stages {
      stage('build') {
        steps {
          withMaven(globalMavenSettingsConfig: 'null', jdk: 'null', maven: 'Maven3', mavenSettingsConfig: 'null') {
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



