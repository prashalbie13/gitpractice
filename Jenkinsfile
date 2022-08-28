pipeline {
       agent any
            stages {
                   stage("git") {
                       steps {  
			       
                            echo 'Downloaded jenkins file from github'
	       }
		   }


                   stage("build") {
			   
                       steps {    
			       echo "BRANCH_HOME"                         
			       echo 'Building the file'
	       }
		   }

                   stage("deploy") {
                       steps {  
			       echo "$BRANCH_HOME" 
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
