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
				sh 'echo "Updating Second Stage"'
				
				when {
					environment name: 'EXECUTE' , value: 'True'
				steps {
					sh 'echo "Step Two"'
				}
			   }
			}
			stage('Third') {
				steps {
					sh 'echo "Step Three"'
				}
			}
		}
}
