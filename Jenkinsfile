pipeline{
	agent none
	stages  {
		stage('Back-end'){
			agent {
				docker {image 'maven:3.8.8-eclipse-temurin-17'}
			}
			steps {
				sh 'mvn --version'
			}
		}
		stage ('front-end') {
			agent {
				docker {image 'node:16-alpine'}
			}
			steps {
				sh 'node --version'
			}
		}
		
	}
}
