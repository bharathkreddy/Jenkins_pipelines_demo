pipeline {
	agent any
	tools {
    	maven 'mav'
	}
	stages {
    	stage("Checkout") {   
        	steps {               	 
            	git url: 'https://github.com/nagenn/testpipe'          	 
           	 
        	}    
    	}
    	stage('Build') {
        	steps {
        	sh "mvn compile"  	 
        	}
    	}
   	 
    	stage("Unit test") {          	 
        	steps {  	 
            	sh "mvn test"          	 
       	}
}
}
}
