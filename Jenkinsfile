pipeline {
	agent any

	triggers {
		pollSCM 'H/1 * * * *'
	}

	options {
		disableConcurrentBuilds()
		timeout(time: 30, unit: 'MINUTES')
	}

	stages {

		stage('Build') {
			sh 'npm install'
		}
//		stage('Building image') {
//			docker.withRegistry( 'https://' + registry, registryCredential ) {
//				def buildName = registry + ":$BUILD_NUMBER"
//				newApp = docker.build(buildName)
//				newApp.push()
//			}
//		}
//		stage('Registring image') {
//			docker.withRegistry( 'https://' + registry, registryCredential ) {
//				newApp.push 'latest2'
//			}
//		}
	}
}
