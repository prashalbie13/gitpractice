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
	
	always {
	echo 'inside always'
	}
       }
