pipeline {
  agent any
  stages {
	  stage('BUILD') {
      steps {
        echo "This is Build stage" 
      }  
    }  
    stage('TEST PARALLELE') {
      parallel {
      stage("TEST ON INTERNET EXPOLRER") {
      steps {
        echo "This is Test on INTERNET EXPOLRER"
      }  
    }  
        stage("TEST ON FIREFOX") {
      steps {
        echo "This is Test on FIREFOX" 
      }  
    }
		stage('Final Test') {
		steps {
		echo "Final Test on Chrome"
		}
		}
    }
    }
    stage ('DEPLOY') {
      steps {
        echo "This is Deploy stage" 
	      echo "Mission"
	      sh 'sleep 5'
      }  
    }
  }
}
