pipeline {
       agent any
            stages {
                   stage("git") {
                       steps {  
			       echo "$BRANCH_HOME" 
                            echo 'Downloaded jenkins file from github'
	       }
		   }


                   stage("build") {
			   
			   when {
				   
				   expression {
				   env.BRANCH_HOME == 'master'
				   }
			   
			   }
                       steps {    
			       echo "$BRANCH_HOME"                         
			       echo 'Building the file'
	       }
		   }

                   stage("deploy") {
                       steps {                          
                            echo 'Deploying'
	       }
		   }

}
	post {
	success {
	echo 'inside always'
	}
       }
}
