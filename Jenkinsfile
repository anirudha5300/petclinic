pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm install petclinic  --set image.repository=registry.hub.docker.com/aniruddha530/tomcat-image --set image.tag=1  --generate-name'
              			
            }           
        }
    }
}
