pipeline {
	agent any
		stages {
			stage('First') {
				environment {
					EXECUTE = 'True'
				}
				steps {
					sh 'echo "Step One"'
					sh 'echo${EXECUTE}'
				}
			}
			stage('Second') {
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
