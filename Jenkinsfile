pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
		checkout scm
	    }
	}
	stage('Build') {
	    steps {
		sh '/home/sandeep/Downloads/apache-maven-3.6.1 /bin/mvn install'
	}
	    }
	stage('Deployment') {
	    steps {
		sh 'cp target/gamutkart.war /home/sandeep/Downloads/apache-tomcat-8.5.42/webapps '
		
	    }
	}

    }
}
