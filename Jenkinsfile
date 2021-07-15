pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					script { env.EXECUTE="True"
						echo ${"Updating second stage"}
						
				      }
				}
			}
			when {
				EXECUTE = "True"
				
			stage('Second') {
				steps {
					script { env.EXECUTE="True"
						
				      }
				}
			} 
	           }
			stage('Third') {
				steps {
					script { echo ${VARIABLE}
				      }
				}
			}
		}
}
