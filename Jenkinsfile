node('maven') {
	
   stage('SCM') {
      // git clone
	  git 'https://github.com/nkr275/spring-petclinic-1.git'
   }
   
    stage ('JUnit test') {
     // publish JUnit test results report
	 junit 'target/surefire-reports/*.xml'
   }
}
