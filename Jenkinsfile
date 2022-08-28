pipeline {
       agent any
            stages {
                   stage("git") {
                       steps {                          
                            echo 'Downloaded jenkins file from github'
	       }
		   }


                   stage("build") {
			   echo "$BRANCH_HOME"
			   when {
				   
				   expression {
				   env.BRANCH_HOME == 'master'
				   }
			   
			   }
                       steps {    
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
