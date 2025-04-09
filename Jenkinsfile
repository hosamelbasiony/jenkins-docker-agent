pipeline {
   agent none

    stage('Cloning Git') {
	    steps{
	      sh 'echo checking out source code'
	    }  
     }  
 
    stage('SAST'){
	agent {
            dockerfile {
            filename 'Dockerfile'
        }
      steps{
      	sh 'echo SAST stage'
	   }
    }
}
}
