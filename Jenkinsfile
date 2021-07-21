pipeline {
			agent any  
			stages {
				stage('STAGE1') {						
					         steps {
							 catcherror(buildResult: 'SUCESS',stageResult: 'FAILURE') {
						sh '''
							pwd
							sleep 5
							exit 1
						'''
							 }
						 }	
				           }
				stage('STAGE2') {						
					         steps {
						sh '''
							echo stage2 is building
							sleep 5
						'''
						 }	
				           }
			}
}
