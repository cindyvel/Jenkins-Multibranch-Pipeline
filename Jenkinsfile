pipeline {
	agent any
	environment {
					EXECUTE = 'True'
				}
		stages {
			stage('First') {
				steps {
					sh 'echo "Step One"'
				}
			}
			stage('Second') {
				when {
					environment name: 'EXECUTE' , value: 'True'
				}
				steps {
					sh 'echo "Updating Second Stage"'
				     }
			}
			stage('Third') {
				when {
					environment name: 'EXECUTE' , value: 'False'
				}
				steps {
					sh 'echo "Step Three"'
				     }
			}
		}
}
