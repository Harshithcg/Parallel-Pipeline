pipeline {
  agent any
  stages {
	  stage ('BUILD') {
      steps {
        echo "This is Build stage" 
      }  
    }  
    stage ('TEST PARALLELE') {
      parallel {
      stage ("TEST ON INTERNET EXPOLRER") {
      steps {
        echo "This is Test on INTERNET EXPOLRER"
      }  
    }  
    }
    }
  }
}
