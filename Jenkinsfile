pipeline {
       agent any
            stages {
                   stage("git") {
                       steps {                          
                            echo 'Downloaded jenkins file from github'
	       }
		   }


                   stage("build") {
			   when {
				   expression {
				   BRANCH_HOME == 'master'
				   }
			   
			   }
                       steps {    
			    sh './test.sh'
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
