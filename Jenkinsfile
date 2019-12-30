node('maven') {
	
   stage('SCM') {
      // git clone
	  git 'https://github.com/nkr275/spring-petclinic-1.git'
   }
   
      
   stage ('build the packages') {
      // mvn  package
	  sh 'mvn clean package'
   }

   
   
   stage ('archival') {
     // archiving artifacts
	 archive 'target/*.jar'

   }
stage ('JUnit test') {
     // publish JUnit test results report
	 junit 'target/surefire-reports/*.xml'
   }
}
