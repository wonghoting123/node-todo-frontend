pipeline {
	agent any

	triggers {
		pollSCM '* * * * *'
	}

	options {
		disableConcurrentBuilds()
		timeout(time: 30, unit: 'MINUTES')
	}

	stages {

		stage('Build') {
			steps {
				sh 'echo 1'
				sh 'echo 2'
				sh 'echo 3'
			}
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
