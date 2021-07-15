pipeline {
	agent any
		stages {
			stage('First') {
				environment {
					EXECUTE = 'True'
				}
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
				steps {
					sh 'echo "Step Three"'
				}
			}
		}
}
