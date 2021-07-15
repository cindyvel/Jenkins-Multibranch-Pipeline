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
			
			stage('Second') {
				when {
				beforeInput true
			  
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
