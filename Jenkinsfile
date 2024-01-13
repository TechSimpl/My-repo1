pipeline {
 agent any
 parameters {
  string( name: 'version', defaultValue: '1.0', description: ' this is version number')
  choice( name: 'env', choices: ['dev', 'qa', 'uat', 'prd'] , description : ' these values are for different envirnments')
  }
  stages {
   stage ('Build') {
    steps {
          //commands rlated to building the code
		  echo " This is build stage"
		  echo " This is build stage for version : ${params.version} "
		  echo " This is build number ${BUILD_NUMBER}"
		  
		  }
 
    }
   stage('deploy ') { 
    steps {
        // COmmands related to code deployment
		  echo " This is deploy stage"
		  echo " This is deploy stage for envirnment : ${params.env}"
	          echo " Build url is ${JOB_DISPLAY_URL}"
		  }
    }
   stage('test') {
    steps {
     // commands related to testing
	      echo " This is deploy stage"
		  }
       }
    }
}

// dummy commit check
